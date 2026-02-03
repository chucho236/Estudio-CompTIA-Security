# ⚖️ Análisis de Seguridad: El Triángulo del Riesgo

Para pasar el Security+, es vital distinguir estos tres conceptos. No son sinónimos, son dependientes.

## 1. Vulnerabilidad (El Punto Débil) 🕳️
Es una debilidad técnica, física o administrativa que puede ser explotada.
* **Ejemplo en mi Lab:** Tener servicios de DNS por defecto (`systemd-resolved`) que no filtran contenido malicioso. 
* **En el examen:** Se mitigan con **Controles** (parches, configuraciones, AdGuard).

## 2. Amenaza (El Agente Externo) ☣️
Cualquier evento o persona con el potencial de explotar una vulnerabilidad.
* **Ejemplo en mi Lab:** Un servidor de **Malware** o un **Script Kiddie** lanzando escaneos automáticos.
* **En el examen:** No las puedes eliminar, solo las puedes **identificar** y monitorear.

## 3. Riesgo (El Impacto Real) ⚠️
Es la probabilidad de que una amenaza encuentre una vulnerabilidad y cause daño.
* **Fórmula:** $Riesgo = Amenaza \times Vulnerabilidad$.
* **Ejemplo en mi Lab:** Si navego en sitios de streaming (Amenaza) sin AdGuard (Vulnerabilidad), el Riesgo de infección por Ransomware es alto.

---

## 🛠️ Práctica: Gestión del Riesgo
En ciberseguridad profesional, una vez que identificas el riesgo, decides qué hacer con él:

1.  **Mitigar:** Poner un control (Instalé **AdGuard Home** para reducir la probabilidad).
2.  **Transferir:** Pasar el riesgo a otro (Contratar un seguro o usar la nube de **Azure**).
3.  **Aceptar:** El riesgo es tan bajo que no vale la pena gastar dinero (Ej. Un ataque dirigido de una nación-estado contra mi lab personal).
4.  **Evitar:** Dejar de hacer la actividad (Apagar el servidor y no entrar a internet).

> **Nota para el examen:** CompTIA pregunta mucho sobre cuál de estas 4 acciones es la más adecuada según el escenario.
