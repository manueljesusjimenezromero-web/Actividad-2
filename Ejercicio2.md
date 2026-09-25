**Experimento de integracion**:

Escenario A:

<img width="787" height="402" alt="Captura de pantalla 2026-09-24 090248" src="https://github.com/user-attachments/assets/e3e0b9e8-f01d-4929-9ea4-db8f0ab11fe1" />

Escenario B

<img width="850" he<img width="837" height="107" alt="Captura de pantalla 2026-09-25 091212" src="https://github.com/user-attachments/assets/6ca166ee-b62b-4230-aecc-31305c571c7d" />

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

Tarda 5,085 Segundos.

En este escenario, bloquea el parseo, haciendo que la página no se vea hasta que los scripts terminen. Esto provoca un mal rendimiento, pero garantiza un orden de ejecución.

<img width="1337" height="290" alt="Captura de pantalla 2026-09-25 091107" src="https://github.com/user-attachments/assets/369ff867-ed38-4917-911e-5efd9ac3ee5a" />

**Escenario B**

Tarda 5,058 Segundos.

No bloquea el parseo, permite ver el contenido rápidamente y los scripts se ejecutan después del DOM, pero antes del evento, con un orden de ejecución.

<img width="1435" height="413" alt="Captura de pantalla 2026-09-25 091755" src="https://github.com/user-attachments/assets/64c1a853-97dc-4e25-b49b-79944e204afb" />

**Escenario C**

Tarda 5,089 Segundos.

No bloquea el parseo, permite ver el contenido rápidamente y los scripts se ejecutan después del DOM, pero antes del evento, con un orden de ejecución.
