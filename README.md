# Operador de telecomunicaciones Interconnect.

Al operador de telecomunicaciones Interconnect le gustaría poder pronosticar su tasa de cancelación de clientes.
Si se descubre que un usuario o usuaria planea irse, se le ofrecerán códigos promocionales y opciones de planes
especiales. El equipo de marketing de Interconnect ha recopilado algunos de los datos personales de sus cliente
incluyendo información sobre sus planes y contratos.

### Descripción de los datos

Los datos consisten en archivos obtenidos de diferentes fuentes:

- `contract.csv` — información del contrato;
- `personal.csv` — datos personales del cliente;
- `internet.csv` — información sobre los servicios de Internet;
- `phone.csv` — información sobre los servicios telefónicos.

En cada archivo, la columna `customerID` (ID de cliente) contiene un código único asignado a cada cliente. La información del contrato es válida a partir del 1 de febrero de 2020.

### Aclaración: Resumen

Característica objetivo: la columna `'EndDate'` es igual a `'No'`.

Métrica principal: AUC-ROC.

Métrica adicional: exactitud.

Criterios de evaluación:

- AUC-ROC < 0.75 — 0 SP
- 0.75 ≤ AUC-ROC < 0.81 — 4 SP
- 0.81 ≤ AUC-ROC < 0.85 — 4.5 SP
- 0.85 ≤ AUC-ROC < 0.87 — 5 SP
- 0.87 ≤ AUC-ROC < 0.88 — 5.5 SP
- AUC-ROC ≥ 0.88 — 6 SP

<!-- TODO: Toma tu ipynb y sepáralo en múltiuples archivos, para modularizar tu código. Usa archivos .py, como expliqué en clases y en estos dos videos: https://www.youtube.com/watch?v=rPEyYGG-w3s - https://www.youtube.com/watch?v=MY4nMmF8gOU -->
<!-- TODO: Una vez que todo esté modularizado, en tu README pon qué pasos debe seguir el usuario para reproducir tu proyecto. Qué setup tiene que hacer y qué línea de código en la terminal le servirá para ejecutar qué cosa? -->
