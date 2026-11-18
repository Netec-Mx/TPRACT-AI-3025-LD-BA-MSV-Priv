# Práctica 5. Aprendizaje y evaluación interna

## Objetivo de la práctica:

Al finalizar la práctica, serás capaz de:

- Convertir un material de referencia sobre atención a consultas rurales en una guía breve de inducción.
- Crear cinco preguntas de comprobación con un Tutor de cuestionarios, fundamentadas únicamente en el material proporcionado.
- Resolver y corregir el cuestionario contrastando las respuestas con las reglas originales.

## Duración aproximada:

- 25 minutos

## Tabla de ayuda:

| Parámetro | Valor | Uso |
| --- | --- | --- |
| Entorno | Microsoft Copilot Chat Básico | Desarrollo de la inducción |
| Agente 1 | Asistente de aprendizaje (Learning Coach) | Crear guía de inducción |
| Agente 2 | Tutor de cuestionarios (Quiz Tutor) | Elaborar preguntas y calificar |
| Material del caso | `GUIA-ATENCION-RURAL-01` | Fuente única de las respuestas |
| Audiencia | Personal de nuevo ingreso que atenderá consultas de clientes rurales | Nivel introductorio |
| Formato del cuestionario | 5 preguntas con 4 opciones, una respuesta correcta | Comprobación de aprendizaje |

## Instrucciones

**Escenario de práctica.** El área de capacitación necesita una inducción breve para personal nuevo que atenderá consultas de clientes rurales. Para evitar inventar políticas, trabajarás únicamente con la guía institucional **ficticia** `GUIA-ATENCION-RURAL-01` incorporada a continuación. La guía no representa normativa real de Banco Agrícola. Después crearás un cuestionario de cinco preguntas y comprobarás sus respuestas contra la misma fuente.

### Tarea 1. Crear una guía breve de inducción con el Asistente de aprendizaje (10 minutos)

**Paso 1.** Abrir **Asistente de aprendizaje** (`Learning Coach`) en Copilot Chat e iniciar una conversación nueva. No es necesario acceder a documentos, SharePoint ni archivos internos.

**Paso 2.** Enviar el siguiente prompt completo. El texto bajo `MATERIAL FUENTE` constituye la única guía institucional del escenario didáctico.

**Prompt 1 — Convertir la guía fuente en una inducción breve**

```text
Actúa como asistente de aprendizaje para personal nuevo que atenderá consultas de clientes rurales. Convierte exclusivamente el siguiente texto de capacitación en una guía de inducción breve y clara en español.

MATERIAL FUENTE: GUIA-ATENCION-RURAL-01
Regla 1. Recepción. Escuchar la consulta de la persona y resumir con palabras sencillas lo que necesita antes de responder.
Regla 2. Trato. Utilizar lenguaje claro, cordial y respetuoso. Evitar tecnicismos que la persona no haya solicitado.
Regla 3. Protección de información. No solicitar contraseñas, códigos de autenticación, números completos de cuenta ni documentos personales mediante un chat o canal no autorizado.
Regla 4. Información de productos. No afirmar tasas, comisiones, plazos, requisitos, elegibilidad o aprobaciones cuando no estén confirmados en información institucional vigente.
Regla 5. Consultas que requieren confirmación. Ante dudas sobre condiciones de un producto, orientar a la persona para que verifique la información por un canal oficial autorizado. No inventar teléfonos, correos ni direcciones web.
Regla 6. Registro. Registrar únicamente el tema general de la consulta en la herramienta autorizada por la organización; no utilizar archivos o notas personales para almacenar datos del cliente.
Regla 7. Escalamiento. Si no hay una respuesta verificada, indicar que se requiere consulta o derivación por un canal autorizado. No improvisar una solución ni prometer resultados.
Regla 8. Cierre. Resumir el siguiente paso permitido y comprobar si la persona comprendió la orientación entregada.

INSTRUCCIONES DE SALIDA
Crea una guía breve para inducción de nuevos colaboradores, de máximo 350 palabras, con título, propósito y secciones organizadas de manera comprensible. Incluye un ejemplo corto de cómo responder a una consulta cuando una tasa o condición no esté verificada, sin inventar datos del banco. Conserva el sentido y las ocho reglas de origen.

No agregues procesos bancarios, leyes, sistemas, obligaciones ni requisitos nuevos. No afirmes que este material es una política real de Banco Agrícola. Devuelve solo la guía de inducción.
```

**Paso 3.** Comparar la guía generada con las ocho reglas del prompt. Confirmar que aborda recepción, trato, protección de información, productos, confirmación por canales oficiales, registro, escalamiento y cierre.

**Paso 4.** Utilizar el siguiente prompt correctivo si algún aspecto se omitió o el agente creó políticas nuevas.

**Prompt 2 — Revisar fidelidad a las ocho reglas**

```text
Revisa la guía de inducción que acabas de generar y compárala con las ocho reglas del material GUIA-ATENCION-RURAL-01 que te proporcioné. Mantén cubiertas las ocho sin inventar procedimientos, direcciones, condiciones bancarias o compromisos. El ejemplo debe limitarse a explicar que una tasa o condición debe confirmarse por los canales oficiales. Devuelve una guía corregida de máximo 350 palabras.
```

**Paso 5.** Conservar la guía breve revisada para utilizarla como apoyo de estudio. Las ocho reglas incluidas en el prompt original permanecen como referencia principal para comprobar las preguntas.

### Tarea 2. Crear cinco preguntas de comprobación con el Tutor de cuestionarios (10 minutos)

**Paso 1.** Abrir **Tutor de cuestionarios** (`Quiz Tutor`) en Copilot Chat e iniciar una conversación nueva. Al cambiar de agente, volver a suministrar el material de referencia: no suponer que conoce la guía generada por el Asistente de aprendizaje.

**Paso 2.** Enviar el siguiente prompt íntegro.

**Prompt 3 — Generar cuestionario fiel al material**

```text
Actúa como tutor de evaluación para personal nuevo. Crea exactamente cinco preguntas de opción múltiple en español, con cuatro alternativas A, B, C y D y una sola respuesta correcta por pregunta.

El material de evaluación es únicamente este texto:
GUIA-ATENCION-RURAL-01
1. Escuchar la consulta y resumir con lenguaje sencillo lo que la persona necesita antes de responder.
2. Mantener un trato claro, cordial y respetuoso, evitando tecnicismos innecesarios.
3. No solicitar contraseñas, códigos de autenticación, números completos de cuenta ni documentos personales mediante canales no autorizados.
4. No asegurar tasas, comisiones, plazos, requisitos, elegibilidad o aprobaciones que no estén confirmados en información institucional vigente.
5. Remitir dudas sobre condiciones de productos a canales oficiales autorizados, sin inventar teléfonos, correos ni enlaces.
6. Registrar solo el tema general de la consulta en herramientas autorizadas; no guardar datos de clientes en notas o archivos personales.
7. Escalar o derivar consultas sin respuesta verificada mediante canales autorizados; no improvisar soluciones ni prometer resultados.
8. Cerrar resumiendo el siguiente paso permitido y comprobando que la persona entendió.

Formula cinco preguntas distintas que comprueben la aplicación de estas reglas en situaciones de atención, sin requerir información externa. Cada pregunta debe tener una respuesta inequívoca sustentada por al menos una regla. No introduzcas otros procedimientos, requisitos legales ni datos bancarios.

Muestra inicialmente solo las cinco preguntas con sus cuatro opciones. No reveles todavía la clave correcta: espera a que te envíe mis cinco respuestas.
```

**Paso 3.** Revisar que el Tutor haya creado exactamente cinco preguntas, con cuatro opciones cada una y sin exigir conocimientos no contenidos en las ocho reglas.

**Paso 4.** Resolver las cinco preguntas y enviar al Tutor de cuestionarios un mensaje con el número de cada pregunta y la letra elegida. Mantener las cinco respuestas en el mismo mensaje para facilitar una corrección conjunta.

**Paso 5.** Mantener visible el material `GUIA-ATENCION-RURAL-01` del prompt anterior, ya que será el criterio de verificación y no la opinión del agente.

### Tarea 3. Resolver y corregir las preguntas contra el material fuente (5 minutos)

**Paso 1.** Utilizar en la misma conversación el siguiente prompt, después de enviar las cinco respuestas, para obtener la clave y la justificación.

**Prompt 4 — Calificar y justificar con la fuente**

```text
Califica las cinco respuestas que acabo de enviarte para el cuestionario basado en GUIA-ATENCION-RURAL-01. Devuelve una tabla con número de pregunta, mi respuesta, respuesta correcta, resultado y número de la regla que respalda la solución. Explica brevemente por qué es correcta cada respuesta. Usa únicamente las ocho reglas originales; si alguna pregunta no se puede responder sin suposiciones, señálala expresamente para corregirla.
```

**Paso 2.** Verificar manualmente las cinco respuestas correctas y sus justificaciones frente a las ocho reglas de la guía fuente. Detectar opciones ambiguas o afirmaciones que atribuyan procesos reales al banco.

**Paso 3.** Enviar la siguiente instrucción y resolver la pregunta corregida si alguna pregunta es ambigua o su clave no se sustenta en el material.

**Prompt 5 — Corregir preguntas sin respaldo**

```text
Revisa las cinco preguntas y la clave de respuestas contra el texto original GUIA-ATENCION-RURAL-01. Corrige exclusivamente las preguntas cuya respuesta no pueda sustentarse en una de las ocho reglas. Mantén un total de cinco preguntas, cuatro opciones por pregunta y una sola respuesta válida. Identifica la regla que fundamenta cada respuesta. No incorpores información externa.
```

**Paso 4.** Confirmar que el cuestionario definitivo contiene cinco preguntas con respuestas, justificaciones y referencia a reglas del material, sin afirmaciones bancarias no verificadas.

### Resultado esperado

- Una guía breve de inducción de máximo 350 palabras que conserva el sentido de las ocho reglas del texto fuente.
- Un cuestionario de cinco preguntas de opción múltiple, con cuatro opciones cada una.
- Cinco respuestas verificadas con justificación y referencia a la regla correspondiente.
- Ninguna pregunta, respuesta o guía agrega políticas, requisitos, tasas o procedimientos institucionales no incluidos en el material del escenario.

[Volver a la lista de prácticas](../README.md)
