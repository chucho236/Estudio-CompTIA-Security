# 🔒 Protocolos de Red: Seguro vs Inseguro

En ciberseguridad, siempre debemos preferir protocolos que utilicen cifrado (TLS/SSL/SSH).

### ❌ Protocolos Inseguros (Cleartext)
- **Telnet (23):** Envía todo en texto plano. Un atacante puede ver tu contraseña.
- **HTTP (80):** No cifra la navegación.
- **FTP (21):** Transferencia de archivos sin protección.

### ✅ Protocolos Seguros (Encrypted)
- **SSH (22):** Reemplaza a Telnet. Cifra la sesión de administración.
- **HTTPS (443):** HTTP sobre TLS. Protege la privacidad web.
- **SFTP (22):** FTP sobre SSH. Ideal para mover archivos al servidor HP.
- **DNSSEC:** Añade firmas digitales al DNS para evitar engaños (relacionado con AdGuard).

### 🍎 Aplicación en el Lab 236
En mi servidor Ubuntu, he deshabilitado cualquier servicio innecesario y priorizo el uso de SSH para la administración remota, asegurando que ninguna credencial viaje en texto claro por mi red local.
