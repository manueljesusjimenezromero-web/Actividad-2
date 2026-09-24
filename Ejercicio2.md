**Experimento de integracion**:

Escenario A:

<img width="787" height="402" alt="Captura de pantalla 2026-09-24 090248" src="https://github.com/user-attachments/assets/e3e0b9e8-f01d-4929-9ea4-db8f0ab11fe1" />

Escenario B

<img width="850" height="411" alt="Captura de pantalla 2026-09-24 091107" src="https://github.com/user-attachments/assets/dca1a9dc-7a2b-47c2-a97a-ea8c752479dd" />

No bloquea el parseo, permite ver el contenido rápidamente y los scripts se ejecutan después del DOM, pero antes del evento, con un orden de ejecución.

Escenario C

<img width="617" height="376" alt="Captura de pantalla 2026-09-24 091338" src="https://github.com/user-attachments/assets/82120761-cf2d-416f-a23f-48a221261598" />

No bloquea el parseo, permite ver el contenido rápidamente y los scripts se ejecutan después del DOM, pero antes del evento, con un orden de ejecución.

Escenario D

<img width="651" height="387" alt="Captura de pantalla 2026-09-24 091535" src="https://github.com/user-attachments/assets/a13f04a0-d7ab-46ea-b318-6803af724478" />

No bloquea el parseo y respeta el orden de ejecución..

Escenario E

<img width="662" height="392" alt="Captura de pantalla 2026-09-24 092305" src="https://github.com/user-attachments/assets/3b841bae-5b89-413c-bf1b-b6c45eb170c3" />

Se comporta como defer, no bloquea el parseo y garantiza el orden de ejecución.

**Informe de Resultados**

**Escenario A**

Tarda 5,085 Segundos

En este escenario, bloquea el parseo, haciendo que la página no se vea hasta que los scripts terminen. Esto provoca un mal rendimiento, pero garantiza un orden de ejecución.

**Escenario B**
