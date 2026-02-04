# 🔑 Autenticación, Autorización y Gestión de Identidades (IAM)

El control de acceso es el proceso de otorgar o denegar solicitudes específicas de recursos.

## 🛡️ Los 5 Factores de Autenticación
1. **Something you know:** Contraseñas / PINs (Lo más común, pero vulnerable).
2. **Something you have:** Smart cards, Tokens RSA, Apps de autenticación (MFA).
3. **Something you are:** Biometría (Huella, Rostro).
4. **Something you do:** Patrones de escritura o gestos.
5. **Somewhere you are:** Restricción por IP o GPS.

## 📋 Modelos de Control de Acceso
- **MAC (Mandatory Access Control):** El sistema decide (usado en gobiernos/milicia).
- **DAC (Discretionary Access Control):** El dueño del archivo decide quién entra (muy flexible, menos seguro).
- **RBAC (Role-Based Access Control):** El acceso se da por tu puesto (Ej. "Vendedor", "Admin"). Es el estándar en empresas grandes.

## 🍎 Aplicación en el Lab 236
- He configurado llaves SSH (**Algo que tengo**) junto con una frase de paso (**Algo que sé**) para acceder al HP ProDesk, cumpliendo con la autenticación multifactor (MFA) técnica.
