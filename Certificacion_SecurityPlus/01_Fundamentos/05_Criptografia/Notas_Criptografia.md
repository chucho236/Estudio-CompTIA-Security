# 🔐 Criptografía: Protegiendo la Información

La criptografía es la base técnica de la Confidencialidad e Integridad en el modelo CIA.

## 🗝️ Cifrado Simétrico (Symmetric)
- **Concepto:** Una sola llave para cifrar y descifrar.
- **Ventaja:** Muy rápido, ideal para grandes volúmenes de datos.
- **Desventaja:** El intercambio de llaves es inseguro.
- **Ejemplo:** AES.

## 🔓 Cifrado Asimétrico (Asymmetric)
- **Concepto:** Par de llaves (Pública y Privada). Lo que una cifra, la otra lo descifra.
- **Uso:** Intercambio de llaves y firmas digitales.
- **Ejemplo:** RSA, ECC.

## 🧬 Hashing (Integridad)
- **Concepto:** Algoritmo de una sola vía para verificar que los datos no han sido alterados.
- **Colisión:** Cuando dos archivos diferentes dan el mismo hash (muy raro).
- **Ejemplo:** SHA-256, MD5 (ya no es seguro).

## 🛡️ Aplicación en el Laboratorio
- **SSH:** Uso de llaves asimétricas para entrar a mi HP ProDesk sin contraseña.
- **HTTPS:** Certificados SSL/TLS para entrar al panel de AdGuard de forma segura.
