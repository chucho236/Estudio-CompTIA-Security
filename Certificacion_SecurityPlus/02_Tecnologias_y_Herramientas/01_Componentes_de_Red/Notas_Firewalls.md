# 🛡️ Dominio 2.0: Tecnologías y Herramientas
## 01. Firewalls y Control de Tráfico

En esta sección documento los dispositivos físicos y lógicos que protegen el perímetro de mi red.

### 🔥 Tipos de Firewalls
1. **Stateless:** Filtra paquetes individualmente basándose en IP/Puerto.
2. **Stateful:** Monitorea el estado de las conexiones activas. Es más inteligente.
3. **NGFW (Next-Gen):** Inspecciona el tráfico a nivel de aplicación (Capa 7 del modelo OSI).

### 📋 Reglas de Firewall (ACL)
Las reglas se leen de arriba hacia abajo. 
- **Implicit Deny:** Es la regla de oro en ciberseguridad. Si no hay una regla que permita explícitamente el tráfico, el firewall debe bloquearlo por defecto.

### 🍎 Aplicación en el Laboratorio 236
- Uso de **UFW (Uncomplicated Firewall)** en mi Ubuntu Server para permitir solo los puertos necesarios:
  - Puerto 53 (DNS para AdGuard).
  - Puerto 3000 (Gestión de AdGuard).
  - Puerto 22 (SSH para administración remota).
