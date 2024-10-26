# Cilyx MK-V
## Proyecto: Generador de Señales de Reloj y PWM con NE555

Este proyecto consiste en la implementación de un generador de señales de reloj y PWM utilizando el temporizador **NE555**. El circuito permite cambiar entre diferentes rangos de frecuencia y ajustar la frecuencia de salida mediante un potenciómetro. Esto lo hace ideal para la enseñanza y práctica de temas relacionados con sistemas digitales, donde las señales de reloj y PWM son esenciales.

## Objetivo del Proyecto
Desarrollar una tarjeta PCB que sirva como una herramienta educativa para estudiantes de sistemas digitales. La tarjeta permitirá generar señales de reloj ajustables y experimentar con distintos rangos de frecuencia. Además, se proporciona una visualización de la señal a través de LEDs, lo que ayuda a entender la relación entre frecuencia y tiempo de encendido/apagado.

## Listado de Componentes

| Componente        | Valor               | Cantidad | Descripción                                                                 |
|-------------------|---------------------|----------|-----------------------------------------------------------------------------|
| NE555             | -                   | 1        | Temporizador configurado en modo astable para generar la señal de salida.   |
| Resistencia       | 1kΩ                 | 1        | Limita la corriente al LED de encendido.                                    |
| Resistencia       | 330Ω                | 1        | Limita la corriente al LED de señal.                                        |
| Resistencia       | 2.7kΩ               | 1        | Parte del ajuste de la frecuencia del NE555.                                |
| Resistencia       | 47kΩ                | 1        | Parte del ajuste de la frecuencia del NE555.                                |
| Potenciómetro     | 500kΩ               | 1        | Permite ajustar la frecuencia de salida dentro del rango seleccionado.      |
| Condensador       | 100 nF, 10 nF, 1 nF | 1 c/u    | Define el rango de frecuencia junto al interruptor.                         |
| Condensador       | 10 nF               | 1        | Filtra la señal de alimentación del NE555.                                  |
| LED               | -                   | 2        | Uno para indicar encendido y otro para visualizar la señal de salida.       |
| Interruptor       | 1P3T (3 posiciones) | 1        | Cambia entre los rangos de frecuencia usando diferentes condensadores.      |
| Fuente de Alimentación | 5V            | 1        | Suministra voltaje al circuito.                                             |

## Funcionamiento del Circuito

1. **Configuración Astable del NE555**:
   - El temporizador NE555 está configurado en modo astable para generar una señal de onda cuadrada continua en su pin de salida (pin 3).
   - La frecuencia de la señal de salida se determina mediante los valores de las resistencias y los condensadores conectados al NE555.
   - Los valores de las resistencias y el condensador principal en la configuración astable afectan directamente la frecuencia y el duty cycle de la señal.

2. **Selección de Rango de Frecuencia**:
   - El interruptor de 3 posiciones permite cambiar entre tres condensadores de diferentes valores (100 nF, 10 nF y 1 nF), lo cual ajusta el rango de frecuencia de la señal:
     - **100 nF (Posición A)**: Rango de frecuencia de 10 Hz a ~130 Hz.
     - **10 nF (Posición B)**: Rango de frecuencia de 130 Hz a ~1 kHz.
     - **1 nF (Posición C)**: Rango de frecuencia de 1 kHz a ~10 kHz.
   - El usuario puede seleccionar el rango deseado para su experimento.

3. **Ajuste Fino de Frecuencia**:
   - Un potenciómetro de 500kΩ permite ajustar la frecuencia de salida dentro del rango seleccionado, proporcionando una señal de reloj de frecuencia variable.
   - Este ajuste fino es ideal para observar el efecto de diferentes frecuencias en sistemas digitales, como contadores o flip-flops.

4. **Visualización de la Señal**:
   - Un LED de señal (con una resistencia limitadora de 330Ω) está conectado a la salida del NE555 y parpadea según la frecuencia generada. Esto permite una visualización rápida de la señal sin necesidad de un osciloscopio.
   - Además, se incluye un LED de encendido (con una resistencia de 1kΩ) para indicar que el circuito está en funcionamiento.

## Funcionamiento Previsto
El circuito generará una señal de reloj con frecuencia ajustable, útil para sistemas digitales. Cambiando la posición del interruptor, el usuario puede seleccionar el rango de frecuencia deseado. El potenciómetro permite hacer ajustes finos dentro de ese rango, y el LED de señal permite una verificación visual de la salida. Este diseño facilita la comprensión de conceptos de frecuencia y duty cycle, así como la relación entre frecuencia y temporización en circuitos digitales.

El circuito puede emplearse para:
- **Sincronización de Circuitos Digitales**: Proveer una señal de reloj a contadores, flip-flops o microcontroladores.
- **Generación de PWM Básico**: Con pequeños ajustes en los valores de resistencia, también puede utilizarse para generar una señal de PWM simple.
- **Aprendizaje Práctico**: Ideal para estudiantes de electrónica y sistemas digitales para experimentar con señales de temporización.

---

Este proyecto proporciona una base sólida para la enseñanza de conceptos de temporización y señales en sistemas digitales. Además, es una herramienta útil en un laboratorio de electrónica donde los estudiantes pueden explorar de manera práctica los principios de la frecuencia y el duty cycle.

