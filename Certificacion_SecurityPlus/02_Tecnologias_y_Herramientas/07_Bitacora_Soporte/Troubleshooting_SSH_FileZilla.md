# 🛠️ Bitácora de Soporte: Resolución de Conectividad SFTP/SSH

## 🔍 Descripción del Problema
Al intentar conectar el cliente **FileZilla** (PC Windows) con el servidor **HP ProDesk** (Ubuntu Server), la conexión era rechazada repetidamente con el error: `Error: No se pudo conectar al servidor`.

## 🛡️ Conceptos Técnicos Aplicados
1. **SFTP (Secure File Transfer Protocol):** Protocolo que corre sobre SSH (puerto 22 por defecto) para transferir archivos de forma cifrada.
2. **Port Non-Standard:** Práctica de cambiar puertos por defecto para evitar escaneos automáticos de bots (Security through Obscurity).
3. **UFW (Uncomplicated Firewall):** Herramienta de filtrado de paquetes en Ubuntu.

## 🛠️ Pasos de Resolución y Comandos

### 1. Identificación del Puerto Real
Se ejecutó el comando para verificar en qué puerto estaba escuchando el servicio SSH:
`sudo ss -tlpn | grep ssh` o revisando el status del servicio.
**Resultado:** Se descubrió que el servidor escuchaba en el puerto **2222** y no en el 22.

### 2. Apertura del Firewall (UFW)
El Firewall estaba bloqueando las conexiones entrantes al nuevo puerto. Se procedió a dar permiso explícito:
`sudo ufw allow 2222/tcp`
- `sudo`: Permisos de superusuario.
- `ufw allow`: Regla para permitir tráfico.
- `2222/tcp`: Especifica el puerto y el protocolo de transporte.

### 3. Configuración del Cliente (FileZilla)
Se ajustaron los parámetros en el Gestor de Sitios:
- **Protocolo:** SFTP (Indispensable para usar SSH).
- **Host:** `sftp://192.168.1.238`
- **Puerto:** `2222`

## ✅ Lecciones Aprendidas
- **No asumir puertos por defecto:** Siempre verificar la configuración del servicio (`/etc/ssh/sshd_config`).
- **Verificar la cadena de conexión:** El Firewall es la primera barrera; si el servicio está activo pero no hay conexión, lo más probable es que sea una regla de UFW.
- **Documentación:** Mantener registro de cambios de puertos evita bloqueos futuros en la administración de activos.
