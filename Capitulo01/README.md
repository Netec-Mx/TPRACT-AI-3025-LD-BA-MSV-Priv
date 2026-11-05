# Práctica 1. Instrucciones efectivas para situaciones bancarias

## Objetivo de la práctica:

Al finalizar la práctica, serás capaz de:

- Formular una instrucción con rol, contexto, objetivo, formato y restricciones utilizando el Asistente de indicaciones.
- Crear y mejorar una respuesta dirigida a un productor agrícola mediante el Asistente de escritura.
- Comparar dos versiones e identificar datos bancarios que requieren confirmación por un canal institucional.

## Duración aproximada:

- 20 minutos

## Tabla de ayuda:

| Parámetro | Valor | Uso |
| --- | --- | --- |
| Entorno | Microsoft Copilot Chat Básico | Conversaciones de práctica |
| Agente 1 | Asistente de indicaciones (Prompt Coach) | Estructurar el prompt |
| Agente 2 | Asistente de escritura (Writing Coach) | Redactar y revisar la respuesta |
| Perfil destinatario | Productor agrícola que solicita orientación inicial | Contexto del mensaje |
| Alcance autorizado | Orientación general, sin políticas ni condiciones crediticias verificadas | Limitar la respuesta |
| Referencia de entorno | [Setup Guide](../SETUP_GUIDE.md) | Validar acceso antes de comenzar |

## Instrucciones

**Escenario de práctica.** Una productora agrícola ficticia desea modernizar el sistema de riego de su finca y solicita orientación inicial sobre cómo empezar una posible solicitud de crédito. Tu responsabilidad es preparar un mensaje comprensible que distinga la orientación general de los requisitos y condiciones que solo Banco Agrícola puede confirmar. No se ha presentado ni evaluado ninguna solicitud.

### Tarea 1. Explorar el Asistente de indicaciones y construir un prompt completo (8 minutos)

**Paso 1.** Abrir Microsoft Copilot Chat con la cuenta del taller y seleccionar el agente **Asistente de indicaciones** desde **Agentes**. Si no aparece, buscarlo en **Todos los agentes** como `Prompt Coach` o con el nombre habilitado por el cliente. Utilizar la [Setup Guide](../SETUP_GUIDE.md) cuando se requiera verificar el acceso.

**Paso 2.** Introducir en el agente el siguiente mensaje. Su función es mejorar una solicitud inicial insuficiente y convertirla en una instrucción utilizable.

**Prompt 1 — Mejorar la consulta inicial**

```text
Actúa como asesor de redacción de prompts para una capacitación bancaria.

Quiero explicar a una productora agrícola que desea modernizar su sistema de riego cómo obtener orientación inicial sobre una posible solicitud de crédito. Mi instrucción original es: "Dile a un agricultor qué necesita para pedir un crédito".

Reescribe esa instrucción como un único prompt listo para usar con un asistente de escritura. Incluye explícitamente cinco componentes: rol del asistente, contexto de una productora agrícola que desea modernizar su sistema de riego y consulta por primera vez, objetivo de la respuesta, formato de salida y restricciones.

El objetivo es redactar una respuesta breve y comprensible que indique cómo consultar los canales oficiales y verificar los pasos y requisitos aplicables. No afirmes que conozcas los requisitos de Banco Agrícola, no inventes tasas, plazos, garantías, montos, listas de documentos, aprobaciones o promesas de otorgamiento. Si falta información, indícalo y remite a verificación institucional.

Solicita un borrador en español claro, de 100 a 140 palabras, con saludo, orientación general y cierre. Devuelve solo el prompt final, sin redactar todavía el mensaje al productor.
```

**Paso 3.** Examinar la instrucción propuesta y localizar sus cinco componentes. Confirmar que contiene una prohibición explícita de inventar requisitos y condiciones de productos bancarios.

**Paso 4.** Utilizar en la misma conversación la siguiente instrucción si el texto carece de algún componente o introduce condiciones crediticias como si estuvieran verificadas.

**Prompt 2 — Ajustar el prompt generado**

```text
Revisa el prompt que acabas de crear. Comprueba, uno por uno, rol, contexto, objetivo, formato y restricciones. Si falta algún componente, incorpóralo. Elimina cualquier requisito, tasa o condición crediticia que parezca una política real del banco sin estar respaldada por una fuente suministrada. Devuelve una sola versión corregida, lista para copiar al Asistente de escritura.
```

**Paso 5.** Copiar el prompt final de la conversación. Conservarlo para utilizarlo directamente en la siguiente tarea; no se necesita crear un archivo externo.

### Tarea 2. Crear y mejorar la respuesta con el Asistente de escritura (8 minutos)

**Paso 1.** Abrir **Asistente de escritura** (`Writing Coach`) desde la sección de agentes de Copilot Chat e iniciar una conversación nueva.

**Paso 2.** Pegar y enviar el prompt final producido en la tarea 1. Leer la primera respuesta generada y conservar visualmente esa versión en la conversación como **versión inicial**.

**Paso 3.** Identificar si el mensaje incluye un saludo, una explicación sencilla, una forma de obtener información oficial y un cierre. Localizar cualquier afirmación que no esté sustentada, como tasas, plazos, elegibilidad automática, documentos obligatorios o garantía de aprobación.

**Paso 4.** Enviar en la misma conversación con el Asistente de escritura la siguiente instrucción de refinamiento.

**Prompt 3 — Mejorar el borrador dirigido al productor**

```text
Revisa el primer mensaje que acabas de redactar para el productor agrícola y genera una versión corregida.

Mantén un trato cordial y fácil de entender. Conserva entre 100 y 140 palabras, con saludo, un párrafo de orientación y un cierre. Conserva el contexto de la modernización del riego. Explica que la información sobre productos, requisitos y condiciones debe confirmarse directamente por los canales oficiales correspondientes antes de dar un paso o entregar documentación.

Elimina cualquier tasa, monto, plazo, lista de documentos, promesa de aprobación o criterio de elegibilidad que no provenga de información institucional verificada. No presentes como política oficial ninguna suposición. Entrega solo la segunda versión del mensaje.
```

**Paso 5.** Confirmar que la nueva respuesta mantiene el objetivo y que evita afirmaciones no verificadas. No enviar los textos a destinatarios reales.

### Tarea 3. Comparar las versiones e identificar información por validar (4 minutos)

**Paso 1.** Mantener visible la conversación con las dos versiones del mensaje y enviar el siguiente prompt para apoyar la comparación.

**Prompt 4 — Comparar sin inventar hechos**

```text
Compara el primer mensaje de esta conversación con la versión corregida. Devuelve una tabla breve con tres columnas: aspecto, primera versión y segunda versión. Revisa claridad, tono, orientación general y restricciones sobre información crediticia. Después, señala qué datos tendría que confirmar una persona con fuentes oficiales antes de convertir el borrador en una comunicación bancaria: requisitos aplicables, condiciones, canales vigentes y plazos, solo si corresponden. No inventes los datos pendientes.
```

**Paso 2.** Comprobar manualmente que la comparación refleja los textos visibles y no atribuye al banco decisiones, condiciones ni procesos que no se hayan proporcionado.

**Paso 3.** Seleccionar la versión que cumple el objetivo y conservar el prompt mejorado junto con la respuesta revisada en la conversación del laboratorio. Considerar explícitamente pendientes de verificación todos los datos específicos del producto o del banco.

### Resultado esperado

- Un prompt utilizable que contiene rol, contexto, objetivo, formato y restricciones.
- Dos versiones distinguibles de una respuesta a un productor agrícola y una versión final comprensible.
- Una comparación verificable que identifica las afirmaciones no sustentadas y deja sin completar los requisitos, tasas y demás condiciones bancarias no proporcionadas.
- La respuesta final no promete un crédito, no inventa requisitos y remite a verificación institucional.

[Volver a la lista de prácticas](../README.md)
