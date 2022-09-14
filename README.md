# KY-040-Rotary-Encoder

¿Qué es el sensor KY-040?
El Módulo KY-040 es un Encoder rotativo es un codificador incremental con dos salidas desfasadas que nos indicará la dirección en la que se está girando el eje. Cuenta con 12 posiciones (cada 30º) e infinito, es decir, que podemos dar vueltas hacia ambos lados sin límite. Cuando pasamos por cada paso se nota un pequeño resalte que indica que se ha llegado a la nueva posición.

!()[http://127.0.0.1:5500/proyecto/Sistemas%20Programables/exposicion-sensor/img/Sensor%201.jpg]

¿Para qué sirve el KY-040?
Este Encoder rotatorio es ampliamente utilizado en el control de motores paso a paso, servomotores, control de potenciómetros digitales, controles de máquinas industriales tales como los husillos de tornos y fresadoras CNC, brazos robóticos, controles de instrumentos electrónicos (diales) y hasta es posible verlos todavía en los viejos ratones de computadoras o en algunos TrackBall.

Especificaciones y características:
+ Voltaje de Alimentación: 5v
+ Corriente: 10 mA
+ Desfase entre señal A y B: 90°
+ Rotación Angular: 30°
+ Ciclos por Resolución (CPR): 20
+ Dimensiones: 20 x 30 x 30 mm
+ Peso: 9 g

¿Cómo funciona el KY-040 Encoder rotativo?
El funcionamiento del codificador rotativo es muy sencillo, al girar el eje del Encoder incremental se generan dos señales cuadradas llamadas canal A (CLK) y B (DT), si el pin común es puesto a masa y el canal A y B con resistencias de Pull Up a VCC, las señales A y B generan pulsos que están desfasadas 90 grados y su secuencia, esto se conoce como código Grey de 2 bits.

Estos codificadores constan de dos pines para el pulsador (funciona como un pulsador normal) y tres pines para el codificador. Los tres pines del codificador van conectados uno a masa y los otros dos a las respectivas entradas que designemos en la placa Arduino. Estas dos señales que salen del encoder nos dan un total de 4 combinaciones. 00, 01, 10, y 11. Esto se conoce como 2 bits de código Grey.
