# CILYX-Mark-V
## Fuente de Alimentación Adaptable para Protoboard

### Introducción
Este proyecto tiene como objetivo construir una fuente de alimentación adaptable para protoboard, de tamaño compacto y fácilmente transportable. Este dispositivo permite seleccionar entre varios niveles de voltaje de salida, como 3.3V, 5V, 12V y un voltaje variable que oscila entre 1V y 11V.

### Especificaciones Técnicas [Que queremos]

- **Tensión de alimentación**: 5V & 12V DC
- **Corriente de salida**: 1A
- **Voltajes de salida fijos**: 3.3V, 5V, 12V DC
- **Voltaje de salida variable**: 1 – 11V DC

### Esquemático Electrónico
A continuación, se detalla el esquema del circuito con los componentes principales:

| Componente           | Descripción                                    |
|----------------------|------------------------------------------------|
| **U1**               | Regulador de voltaje SMD (AMS 1117-3.3) - 3.3V |
| **U2**               | Regulador de voltaje SMD (AMS 1117-5.0) - 5.0V |
| **J1**               | Jack USB 2 Tipo B                              |
| **J2**               | Borneras de conexión 2 pines                   |
| **J3**               | Jack power 12V                                 |
| **J4, J8**           | Pines espadines Macho                          |
| **D1**               | Diodo Schottky SS14-T                          |
| **D2-D5**            | LED verde SMD (Paquete 1206)                   |
| **R1, R2, R5-R6**    | Resistencia SMD 1/4W 1k Ohm (Paquete 1206)     |
| **R3-R4**            | Resistencia SMD 1/4W 330 Ohm (Paquete 1206)    |
| **RV1**              | Potenciómetro de precisión                     |
| **C1, C2, C5**       | Capacitor cerámico 0.1µF (Paquete 1206)        |
| **C3, C4, C6**       | Capacitor electrolítico 10µF 16V               |

<!-- ### Descargar Diseño-->

<!-- - **Diseño Esquemático en Proteus 8.9**: [Descargar aquí](#) <!-- Inserta el enlace adecuado -->
<!-- - **Diseño de la Tarjeta PCB**: [Ordena ahora en JLCPCB](https://jlcpcb.com) <!-- Inserta el enlace adecuado -->

### Instrucciones de Uso [Segun lo que tengo en la mente]
1. Conectar la fuente de alimentación a una entrada de 5V o 12V, dependiendo de los requerimientos de tu proyecto.
2. Elige el nivel de voltaje adecuado para tu circuito (3.3V, 5V, 12V o un voltaje variable entre 1V y 11V) mediante switches.
3. Monta los componentes en la protoboard y conéctalos a la salida de la fuente de alimentación para verificar el correcto funcionamiento del circuito.

### Notas adicionales
Este diseño es ideal para proyectos pequeños donde se requiere movilidad y flexibilidad en los niveles de voltaje, evitando el uso de fuentes de alimentación grandes y poco portátiles.
