# Práctica 2. Comunicaciones claras para clientes agrícolas

## Objetivo de la práctica:

Al finalizar la práctica, serás capaz de:

- Redactar un correo claro y cordial con el Diseñador de comunicaciones corporativas.
- Convertir el correo en un recordatorio breve mediante el Asistente de escritura.
- Traducir la comunicación con el Traductor de texto y verificar su sentido, tono y terminología.

## Duración aproximada:

- 25 minutos

## Tabla de ayuda:

| Parámetro | Valor | Uso |
| --- | --- | --- |
| Plataforma | Microsoft Copilot Chat Básico | Acceso a las conversaciones de los agentes |
| Agente de correo | Diseñador de comunicaciones corporativas (`Corporate Communications Crafter`) | Redactar la comunicación |
| Agente de recordatorio | Asistente de escritura (`Writing Coach`) | Reducir y ajustar el mensaje |
| Agente de traducción | Traductor de texto (`Text Translator`) | Traducir y revisar |
| Destinataria ficticia | María Robles | Identificar a la persona del caso |
| Referencia del caso | `CASO-MR-02` | Mantener la misma referencia en los tres textos |
| Información pendiente | Presupuesto actualizado de insumos y calendario estimado de cobros | Únicos elementos por solicitar en el ejercicio |
| Idioma de destino | Inglés | Simular la preferencia lingüística de la destinataria |

> **Importante:** Los documentos pendientes se definieron exclusivamente para este ejercicio; **no son requisitos oficiales** de Banco Agrícola. No se enviarán correos ni se usará información de clientes reales. Los agentes deben estar habilitados previamente, como explica la [Setup Guide](../SETUP_GUIDE.md).

## Instrucciones

**Escenario de práctica.** María Robles, productora agrícola ficticia, presentó una consulta preliminar relacionada con su próxima campaña. El equipo recibió una descripción inicial, pero necesita solicitar dos elementos acordados para completar el expediente didáctico. Se requiere un correo respetuoso, un recordatorio conciso y una versión en inglés, sin añadir condiciones, plazos o requisitos institucionales.

### Tarea 1. Elaborar un correo claro con el Diseñador de comunicaciones corporativas (10 minutos)

**Paso 1.** Abrir el agente **Diseñador de comunicaciones corporativas** desde **Agentes** en Microsoft Copilot Chat y comenzar una conversación nueva. Confirmar que es el agente autorizado para el taller.

**Paso 2.** Enviar el siguiente prompt con todos los datos del caso.

**Prompt 1 — Correo de solicitud de información pendiente**

```text
Actúa como asistente de comunicaciones de un equipo de atención agrícola en un ejercicio de capacitación.

Redacta un correo en español para María Robles, productora agrícola ficticia, con referencia CASO-MR-02.

Hechos autorizados:
- Ya se recibió una descripción inicial de su proyecto para la próxima campaña.
- Para el expediente didáctico solo faltan dos elementos previamente acordados: presupuesto actualizado de insumos y calendario estimado de cobros.
- No existe plazo de entrega definido ni se ha evaluado una solicitud bancaria.
- La destinataria prefiere recibir también una versión del mensaje en inglés.

Formato: asunto, saludo, cuerpo breve, lista de los dos elementos pendientes y despedida. Longitud: 110 a 150 palabras. Tono profesional, cordial y directo.

No inventes otros documentos, correos, teléfonos, enlaces, plazos, tasas, condiciones, requisitos oficiales ni decisiones de aprobación. No presentes los dos elementos del ejercicio como políticas del banco. Indica que el canal autorizado de entrega debe confirmarse antes de remitir documentos. Devuelve solamente el correo.
```

**Paso 3.** Comprobar que el correo contiene asunto, referencia `CASO-MR-02`, los dos elementos pendientes y una solicitud cordial, sin fecha límite ni requisitos adicionales.

**Paso 4.** Enviar esta corrección si se altera el caso, sin reiniciar toda la actividad.

**Prompt 2 — Corregir datos y tono**

```text
Corrige el correo anterior: el caso es CASO-MR-02 y solo se solicitan el presupuesto actualizado de insumos y el calendario estimado de cobros, definidos para el ejercicio. Elimina cualquier otro documento, plazo, canal concreto, condición bancaria o promesa. Conserva asunto, saludo, lista y despedida. Devuelve únicamente el correo corregido.
```

**Paso 5.** Copiar el correo revisado para reutilizarlo en las tareas siguientes. Conservar la versión final en la conversación o en un documento autorizado si el taller requiere guardar el entregable.

### Tarea 2. Convertir el correo en un recordatorio breve con el Asistente de escritura (7 minutos)

**Paso 1.** Abrir **Asistente de escritura** (`Writing Coach`) e iniciar una conversación nueva.

**Paso 2.** Enviar el siguiente prompt. A continuación, pegar **en un mensaje separado** el correo completo de la tarea 1.

**Prompt 3 — Crear un recordatorio a partir del correo**

```text
Voy a pegar a continuación un correo escrito para María Robles sobre el caso CASO-MR-02. Espera a recibir el correo completo antes de redactar.

Cuando lo recibas, conviértelo en un recordatorio en español de entre 45 y 65 palabras. Conserva el nombre, la referencia CASO-MR-02 y los dos elementos pendientes exactamente como figuran en la fuente. Usa un tono amable y evita presión indebida. No inventes plazos, advertencias, otros documentos, canales de envío, tasas ni condiciones. Entrega solamente el recordatorio.
```

**Paso 3.** Verificar que el recordatorio sigue mencionando los dos elementos pendientes y reduce la longitud sin alterar el sentido.

**Paso 4.** Utilizar esta instrucción correctiva si el agente ha agregado información.

**Prompt 4 — Retirar información agregada**

```text
Revisa el recordatorio y elimina cualquier dato que no figure en el correo fuente. Conserva CASO-MR-02, presupuesto actualizado de insumos y calendario estimado de cobros. No incluyas una fecha límite ni un canal de entrega específico. Devuelve un único mensaje de máximo 65 palabras.
```

### Tarea 3. Traducir el mensaje y comprobar sentido, tono y terminología (8 minutos)

**Paso 1.** Abrir **Traductor de texto** (`Text Translator`) y comenzar otra conversación.

**Paso 2.** Enviar el siguiente prompt y, en el mensaje siguiente, pegar el **correo final en español de la tarea 1**, no el recordatorio.

**Prompt 5 — Traducir el correo al inglés**

```text
Voy a enviarte un correo empresarial ficticio en español. Espera a recibir el texto antes de responder.

Tradúcelo al inglés internacional. Conserva la estructura de correo, el nombre propio María Robles, la referencia CASO-MR-02 y el significado de los dos elementos pendientes. Mantén un tono respetuoso y cordial. No traduzcas el identificador del caso ni agregues requisitos, compromisos, canales, fechas límite o condiciones bancarias. Devuelve únicamente la traducción.
```

**Paso 3.** Comparar manualmente el texto de origen y la traducción: verificar nombre, referencia, ambos elementos pendientes, tono y ausencia de nuevas condiciones. Comprobar especialmente que *budget for inputs* y *estimated collections schedule*, o expresiones equivalentes, conservan su sentido.

**Paso 4.** Solicitar una comprobación de fidelidad con el siguiente prompt.

**Prompt 6 — Revisar significado y terminología**

```text
Compara el correo original en español que te envié con tu traducción inglesa. Señala, de forma breve, cualquier cambio de significado en el destinatario, los dos elementos pendientes, el tono o las restricciones. Si hay un error, devuelve el correo completo en inglés ya corregido. No agregues hechos ni requisitos nuevos.
```

**Paso 5.** Confirmar personalmente que la versión revisada en inglés transmite el mismo contenido. Conservar los tres productos del ejercicio sin enviarlos a contactos reales.

### Resultado esperado

Se dispone de un **correo en español**, un **recordatorio breve** y una **traducción al inglés** del correo. Los tres textos identifican el caso `CASO-MR-02`, conservan exactamente los dos elementos pendientes y no incluyen requisitos oficiales, plazos ni condiciones de crédito que no se hayan aportado.

[Volver a la lista de prácticas](../README.md)
