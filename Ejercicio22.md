Escenarios:

Escenario A:

<img width="787" height="402" alt="Captura de pantalla 2026-09-24 090248" src="https://github.com/user-attachments/assets/e3e0b9e8-f01d-4929-9ea4-db8f0ab11fe1" />

En este escenario, bloquea el parseo haciendo que no ve la pagina hasta que los script terminen, hace que tenga mal rendimiento pero un orden de ejecución garantizado.

Escenario B

<img width="850" height="411" alt="Captura de pantalla 2026-09-24 091107" src="https://github.com/user-attachments/assets/dca1a9dc-7a2b-47c2-a97a-ea8c752479dd" />

No bloquea el parseo, dejaría ver el contenido rápido y los scripts se ejecutan después del DOM, pero antes del evento y orden de ejecución garantizado.

Escenario C

<img width="617" height="376" alt="Captura de pantalla 2026-09-24 091338" src="https://github.com/user-attachments/assets/82120761-cf2d-416f-a23f-48a221261598" />

No bloquea el parseo, pero ejecuta en cuanto descarga, el orden no esta garantizado, puede ejecutar código antes de que exista parte del DOM.

Escenario D

<img width="651" height="387" alt="Captura de pantalla 2026-09-24 091535" src="https://github.com/user-attachments/assets/a13f04a0-d7ab-46ea-b318-6803af724478" />

No bloquea el parseo y respeta el orden.

Escenario E

<img width="662" height="392" alt="Captura de pantalla 2026-09-24 092305" src="https://github.com/user-attachments/assets/3b841bae-5b89-413c-bf1b-b6c45eb170c3" />

Se comporta como el defer, no bloquea el parseo, orden garantizado.
