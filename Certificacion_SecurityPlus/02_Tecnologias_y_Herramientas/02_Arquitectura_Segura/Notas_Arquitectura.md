# 🏗️ Arquitectura de Red y Diseño Seguro

El diseño de la red es la primera línea de defensa contra el movimiento lateral de un atacante.

## 1. Segmentación y VLANs
- **Propósito:** Aislar dispositivos por función o nivel de confianza.
- **Beneficio:** Limita el "radio de explosión" (Blast Radius) de un ataque. Si un dispositivo IoT es comprometido, el servidor principal permanece seguro.

## 2. DMZ (Demilitarized Zone)
- Red perimetral que aloja servicios orientados al público (Web, Mail, DNS).
- Actúa como un búfer entre la red interna (confiable) e internet (no confiable).

## 3. Honeypots (Sistemas de Engaño)
- Sistemas diseñados para ser explorados y atacados con el fin de recolectar inteligencia sobre las tácticas del atacante (TTPs).

## 4. Air Gap
- Aislamiento físico total de una red. Es el control de seguridad más fuerte para prevenir ataques remotos.

## 🍎 Aplicación en el Lab 236
- **Estrategia sugerida:** Implementar una subred separada para dispositivos IoT (TV, Celulares) para que no tengan visibilidad directa sobre la interfaz de administración del servidor HP ProDesk.
