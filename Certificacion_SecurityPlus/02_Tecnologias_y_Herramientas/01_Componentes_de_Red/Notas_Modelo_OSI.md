# 🗺️ El Modelo OSI en Ciberseguridad

El Modelo OSI divide la comunicación en 7 capas para facilitar el diagnóstico y la protección.

## 🧱 Las 7 Capas
1. **Aplicación (HTTP, FTP, AdGuard):** Interfaz del usuario.
2. **Presentación (SSL/TLS, JPG):** Formato y cifrado de datos.
3. **Sesión (NetBIOS):** Control de diálogo y gestión de conexiones.
4. **Transporte (TCP, UDP):** Puertos y segmentación.
5. **Red (IP, ICMP):** Direccionamiento lógico y enrutamiento (Routers).
6. **Enlace de Datos (MAC, Ethernet):** Direccionamiento físico (Switches).
7. **Física (Cables, Señal de Radio):** Transmisión binaria.

## 🛡️ Relación con Seguridad
- **Capa 7:** Firewalls de próxima generación (NGFW) y filtros DNS (AdGuard).
- **Capa 4:** Reglas de puertos en UFW / IPtables.
- **Capa 3:** Filtrado por direcciones IP.
- **Capa 2:** Seguridad de puertos en Switches (Port Security).
