# Práctica 4. Acuerdos de reuniones y seguimiento

## Objetivo de la práctica:

Al finalizar la práctica, serás capaz de:

- Convertir una minuta de reunión de varias áreas en acuerdos y responsables comprobables.
- Transformar esos acuerdos en una lista de actividades, prioridades, fechas y estados iniciales mediante el Asistente de scrum.
- Detectar y retirar tareas, aprobaciones y decisiones que no aparecen en la minuta fuente.

## Duración aproximada:

- 25 minutos

## Tabla de ayuda:

| Parámetro | Valor | Uso |
| --- | --- | --- |
| Entorno | Microsoft Copilot Chat Básico | Procesar la minuta y las tareas |
| Agente 1 | Asesor de reuniones (Meeting Coach) | Extraer acuerdos |
| Agente 2 | Asistente de scrum (Scrum Assistant) | Organizar el seguimiento |
| Minuta | `MIN-AGR-04` | Texto fuente del ejercicio |
| Reunión simulada | 22 de octubre de 2026 | Referencia temporal |
| Áreas participantes | Comercial, Riesgos y Operaciones | Responsables permitidos |
| Estado inicial de los acuerdos | Pendiente | Representar tareas aún no ejecutadas |

## Instrucciones

**Escenario de práctica.** Comercial, Riesgos y Operaciones mantuvieron una reunión ficticia para preparar una posible campaña informativa dirigida a productores agrícolas. Se requiere convertir la minuta original en acuerdos y tareas de seguimiento sin confundir los asuntos abiertos con decisiones autorizadas. La campaña todavía **no ha sido aprobada**.

### Tarea 1. Convertir la minuta en acuerdos y responsables con el Asesor de reuniones (10 minutos)

**Paso 1.** Abrir **Asesor de reuniones** (`Meeting Coach`) desde los agentes disponibles en Microsoft Copilot Chat y crear una conversación nueva. No se requiere grabar una reunión ni utilizar Teams.

**Paso 2.** Pegar el siguiente prompt, que contiene la minuta completa de la sesión didáctica.

**Prompt 1 — Estructurar una minuta sin agregar decisiones**

```text
Actúa como asistente de reuniones para estructurar una minuta de capacitación. Usa exclusivamente la información textual que sigue; no consultes calendarios, correos o archivos externos.

MINUTA MIN-AGR-04
Fecha de la reunión simulada: 22 de octubre de 2026.
Participantes: representantes de las áreas Comercial, Riesgos y Operaciones.
Objetivo: coordinar actividades preparatorias para una posible campaña informativa dirigida a productores agrícolas.

ACUERDOS EXPRESOS
A1. Comercial preparará un borrador de preguntas frecuentes para la campaña. Responsable: Comercial. Fecha objetivo: 29 de octubre de 2026. Prioridad acordada: alta.
A2. Riesgos revisará el texto de la invitación para identificar afirmaciones que necesiten validación institucional. Responsable: Riesgos. Fecha objetivo: 30 de octubre de 2026. Prioridad acordada: alta.
A3. Operaciones verificará la capacidad de atención del canal telefónico antes de proponer una fecha de difusión. Responsable: Operaciones. Fecha objetivo: 2 de noviembre de 2026. Prioridad acordada: media.
A4. Comercial consolidará los hallazgos de las tres áreas y preparará un resumen para la siguiente reunión. Responsable: Comercial. Fecha objetivo: 3 de noviembre de 2026. Prioridad acordada: media.

NOTAS SIN APROBACIÓN
La siguiente reunión se prevé para el 4 de noviembre de 2026. No se ha aprobado el lanzamiento de la campaña, el presupuesto, la difusión de mensajes ni la utilización de datos de clientes. La posibilidad de preparar materiales adicionales quedó como tema abierto, sin responsable ni fecha.

Devuelve una minuta estructurada en español con: propósito, cuatro acuerdos A1-A4 en una tabla (actividad, responsable, fecha objetivo, prioridad), decisiones explícitamente no tomadas y asuntos abiertos. No inventes asistentes con nombre, tareas, fechas, aprobaciones, compromisos ni decisiones. No presentes el tema abierto como acuerdo asignado.
```

**Paso 3.** Comprobar que aparecen exactamente los acuerdos `A1`, `A2`, `A3` y `A4`, con los responsables, fechas y prioridades originales.

**Paso 4.** Revisar que el lanzamiento, el presupuesto y el uso de datos de clientes figuren como decisiones no aprobadas; el tema de materiales adicionales debe permanecer como asunto abierto.

**Paso 5.** Enviar el ajuste siguiente si la salida contiene más de cuatro acuerdos.

**Prompt 2 — Corregir la extracción de acuerdos**

```text
Revisa la minuta estructurada anterior contra la transcripción de MIN-AGR-04 que te proporcioné. Solo existen cuatro acuerdos: A1, A2, A3 y A4. No conviertas la reunión futura ni los materiales adicionales en tareas asignadas. No hay decisión de lanzar la campaña, aprobar presupuesto ni utilizar datos de clientes. Elimina cualquier acuerdo o responsable que no esté en el texto fuente. Devuelve la minuta corregida.
```

**Paso 6.** Copiar la tabla final de acuerdos para utilizarla como entrada del siguiente agente.

### Tarea 2. Transformar acuerdos en actividades y estados con el Asistente de scrum (10 minutos)

**Paso 1.** Abrir **Asistente de scrum** (`Scrum Assistant`) e iniciar una conversación nueva. No crear un proyecto ni conectar una herramienta de gestión externa; el resultado será una lista de tareas presentada dentro del chat.

**Paso 2.** Enviar el siguiente prompt y, cuando el agente lo pida, pegar la tabla corregida de cuatro acuerdos obtenida con el Asesor de reuniones.

**Prompt 3 — Construir el tablero de tareas**

```text
Necesito convertir una tabla de cuatro acuerdos de una reunión simulada en una lista de seguimiento de tareas. Te enviaré esa tabla en mi siguiente mensaje; espera a recibirla antes de crear la lista.

Después, genera una tabla Markdown con exactamente estas columnas: identificador, actividad, responsable, fecha objetivo, prioridad y estado inicial. Usa únicamente los acuerdos A1, A2, A3 y A4 recibidos. Conserva literalmente cada responsable, fecha y prioridad indicados; asigna a todas las filas el estado inicial "Pendiente". Ordena las tareas primero por prioridad alta y luego por fecha objetivo.

No inventes dependencias, porcentajes de avance, nuevas fechas, aprobaciones, responsables con nombre propio ni resultados completados. No crees tareas para asuntos sin acuerdo. Devuelve la tabla y una nota breve que aclare que la campaña no está aprobada.
```

**Paso 3.** Pegar como siguiente mensaje la tabla de acuerdos copiada de la tarea 1. Si el agente necesita distinguir un campo, utilizar las etiquetas `A1`, `A2`, `A3` y `A4` incluidas en la salida original.

**Paso 4.** Confirmar que la tabla de tareas contiene cuatro filas, que el estado de todas es `Pendiente`, que las prioridades son dos `alta` y dos `media`, y que las fechas siguen asociadas a sus responsables originales.

**Paso 5.** Enviar el prompt de control siguiente si aparecen tareas o estados no establecidos.

**Prompt 4 — Alinear el tablero con los acuerdos**

```text
Corrige la tabla de tareas para que represente únicamente los acuerdos A1-A4 que te facilité. Todas las actividades comienzan en estado "Pendiente". No agregues tareas de lanzamiento, presupuesto, envío de campañas, consultas de clientes ni materiales adicionales. Conserva actividades, responsables, fechas y prioridades que estaban expresamente en la fuente. Devuelve solo el tablero corregido.
```

### Tarea 3. Verificar las tareas contra la minuta original (5 minutos)

**Paso 1.** Comparar la tabla del **Asistente de scrum** con el texto de la minuta `MIN-AGR-04` que aparece en la tarea 1. Comprobar esta correspondencia:

| Acuerdo | Responsable correcto | Fecha objetivo correcta | Prioridad correcta | Estado inicial esperado |
| --- | --- | --- | --- | --- |
| A1 | Comercial | 29 de octubre de 2026 | Alta | Pendiente |
| A2 | Riesgos | 30 de octubre de 2026 | Alta | Pendiente |
| A3 | Operaciones | 2 de noviembre de 2026 | Media | Pendiente |
| A4 | Comercial | 3 de noviembre de 2026 | Media | Pendiente |

**Paso 2.** Identificar y eliminar cualquier decisión adicional sobre lanzamiento, presupuesto, uso de datos de clientes o actividades asignadas a un área sin acuerdo expreso. Si se requiere corregir la tabla, usar el prompt de la tarea 2.

**Paso 3.** Verificar que la minuta estructurada y la lista de tareas coinciden en identificadores, actividad, responsable, fecha y prioridad, y que ninguna tarea aparece como ejecutada.

### Resultado esperado

- Una minuta estructurada que reconoce los cuatro acuerdos originales y separa los temas abiertos y las decisiones no aprobadas.
- Una lista o tablero de cuatro actividades con responsables, fechas, prioridades y estado inicial `Pendiente`.
- Correspondencia verificable `A1` a `A4` entre la minuta y las tareas, sin decisiones ni resultados agregados por la IA.

[Volver a la lista de prácticas](../README.md)
