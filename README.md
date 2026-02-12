# Variador de Velocidad y Sentido de Giro para Motor DC

## 📝 Descripción
Este proyecto consiste en el diseño e implementación de un sistema de control para motores de corriente continua (12V). Utiliza una técnica de modulación por ancho de pulso (PWM) para el control de velocidad y una etapa de potencia basada en un Puente H discreto para invertir el sentido de giro.

## 🛠️ Especificaciones Técnicas
- **Control de Velocidad:** PWM generado por CI 555 en configuración astable.
- **Etapa de Potencia:** Puente H compuesto por 4 MOSFETs de canal N (IRFZ44N).
- **Protección:** Diodos de libre circulación (Ultra-fast) 1N5408 y aislamiento galvánico mediante optoacopladores.
- **Lógica de Control:** Puertas digitales (AND, OR, NOT) con sistema de enclavamiento (bloqueo) de seguridad.
- **Regulación:** LM1117T para la etapa lógica (5V) a partir de la fuente principal de 12V.

## ⚙️ Características Destacadas
- **Aislamiento Galvánico:** El uso de optoacopladores protege la etapa de control de los picos de corriente y ruido del motor.
- **Bloqueo de Seguridad:** Lógica digital integrada que impide la activación simultánea de ambos sentidos, evitando cortocircuitos en las ramas del puente.
- **Flexibilidad de Potencia:** Incluye un socket para alimentación externa, permitiendo controlar motores de mayor voltaje independientemente de la lógica.

## 🚀 Cómo abrir la simulación
1. Descargar los archivos de la carpeta `/Simulacion`.
2. Abrir con Proteus 8.x o superior.
3. Consultar el PDF en `/Documentacion` para ver los cálculos de diseño.
4. Consultar diseño de la pcb en `/PCB` para ver el diseño fisico en KiCad.
