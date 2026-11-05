# Práctica 3. Preparación de propuestas y respuestas comerciales

## Objetivo de la práctica:

Al finalizar la práctica, serás capaz de:

- Elaborar un borrador comercial con el Generador de solicitudes de propuesta a partir de una ficha ficticia de condiciones.
- Organizar preguntas frecuentes con el Asistente de información disponible, sin presuponer acceso a sistemas bancarios.
- Detectar y corregir afirmaciones sin respaldo, dejando pendientes los aspectos que requieren validación institucional.

## Duración aproximada:

- 25 minutos

## Tabla de ayuda:

| Parámetro | Valor | Uso |
| --- | --- | --- |
| Plataforma | Microsoft Copilot Chat Básico | Generación de contenidos |
| Agente de propuesta | Generador de solicitudes de propuesta (`Request for Proposal Generator`) | Preparar borrador |
| Agente para consultas | Asistente de información disponible (nombre facilitado por el cliente) | Crear preguntas frecuentes |
| Solicitante ficticio | Asociación de Productores Valle Verde | Destinatario de la propuesta |
| Identificador | `FICHA-VV-03` | Referencia única del escenario |
| Servicio ficticio | Servicio Empresarial de Gestión Administrativa Agro | Ejercicio de respuesta comercial; **no acredita la existencia de un producto real** |
| Información no proporcionada | Tarifas, tasas, comisiones, requisitos documentales concretos, condiciones contractuales, plazos y decisiones | Deben quedar pendientes de confirmación |

> **Importante:** La ficha que aparece a continuación es **inventada para el laboratorio** y no representa productos, políticas, requisitos ni ofertas vigentes de Banco Agrícola. No utilizar sistemas, expedientes, cuentas ni datos reales. Verificar previamente los agentes mediante la [Setup Guide](../SETUP_GUIDE.md).

## Instrucciones

**Escenario de práctica.** La Asociación de Productores Valle Verde desea información inicial para coordinar cobros y pagos de sus miembros. El equipo comercial dispone de una ficha ficticia que describe únicamente un servicio de orientación empresarial y sus límites. Deberás preparar una respuesta, organizar posibles preguntas frecuentes y retirar cualquier afirmación no documentada antes de presentar el borrador para revisión.

### Tarea 1. Estructurar una respuesta con el Generador de solicitudes de propuesta (10 minutos)

**Paso 1.** Abrir **Generador de solicitudes de propuesta** en Copilot Chat e iniciar una conversación nueva. No se requiere acceder a catálogos institucionales, contratos ni aplicaciones bancarias.

**Paso 2.** Utilizar la siguiente ficha completa incluida dentro del prompt. Considerarla la única fuente válida del ejercicio.

**Prompt 1 — Propuesta basada en ficha ficticia**

```text
Actúa como redactor comercial de un escenario didáctico. Prepara una respuesta preliminar en español a la Asociación de Productores Valle Verde, sin presentarla como oferta real de Banco Agrícola.

FICHA FICTICIA FICHA-VV-03 — Uso exclusivo de capacitación
Entidad simulada: Banco Agrícola Simulado.
Servicio simulado: Servicio Empresarial de Gestión Administrativa Agro.
Necesidad manifestada: la asociación desea información inicial sobre cómo centralizar la gestión administrativa de cobros y pagos de sus miembros.
Propósito declarado del servicio ficticio: ofrecer orientación inicial sobre alternativas de gestión administrativa de cobros y pagos para organizaciones agropecuarias.
Público descrito en esta ficha ficticia: asociaciones de productores legalmente constituidas.
Actividad prevista: puede proponerse una reunión de orientación de 45 minutos, sujeta a confirmar disponibilidad con el equipo comercial.
Revisión posterior: una eventual solicitud se sometería a revisión interna; no hay aprobación ni contratación garantizada.
Información no disponible: tarifas, tasas, comisiones, requisitos documentales específicos, condiciones contractuales, plazos de respuesta, elegibilidad individual y disponibilidad definitiva.

Genera un borrador breve con: asunto y referencia FICHA-VV-03, saludo, comprensión de la necesidad, explicación limitada del propósito del servicio simulado, condiciones y límites de lo informado, propuesta de reunión sujeta a confirmación y lista final de puntos que deben validar las áreas autorizadas.

Restricciones: usa solo los hechos de esta ficha. No supongas que puedes consultar sistemas bancarios, expedientes, catálogos, agendas o fuentes internas. No inventes tasas, comisiones, tarifas, fechas, productos adicionales, integraciones, requisitos, aprobaciones ni promesas. Distingue siempre lo descrito en este ejercicio de lo pendiente de verificación. No afirmes que el servicio ficticio existe realmente. Devuelve el borrador comercial.
```

**Paso 3.** Revisar que la respuesta contenga las secciones requeridas y que la reunión de 45 minutos sea **una posibilidad sujeta a disponibilidad**, nunca un compromiso confirmado.

**Paso 4.** Solicitar esta corrección si el agente introduce información no sustentada.

**Prompt 2 — Limitar el borrador a la ficha**

```text
Corrige el borrador FICHA-VV-03 usando solo los datos de la ficha ficticia que te facilité. Quita precios, requisitos documentales concretos, integraciones, fechas, aprobaciones o funcionalidades no descritas. Presenta el servicio como un caso simulado y deja lo desconocido como "Pendiente de verificación institucional". Conserva la estructura de la respuesta.
```

**Paso 5.** Conservar el borrador de la propuesta para contrastarlo con las preguntas frecuentes y para la revisión final.

### Tarea 2. Organizar preguntas frecuentes con el Asistente de información disponible (8 minutos)

**Paso 1.** Abrir **Asistente de información disponible** con el acceso previamente facilitado por el cliente e iniciar una conversación nueva. No asumir que conoce el contenido de la otra conversación.

**Paso 2.** Enviar este prompt autónomo, que vuelve a aportar los hechos necesarios del caso.

**Prompt 3 — Seis preguntas frecuentes basadas en la ficha**

```text
Actúa como asistente de consulta de información proporcionada para un ejercicio didáctico. No tienes acceso autorizado a sistemas internos, expedientes, productos, precios, calendarios ni documentos del banco. Trabaja solo con los hechos incluidos aquí.

FICHA-VV-03 — Entidad: Banco Agrícola Simulado.
Solicitante: Asociación de Productores Valle Verde.
Servicio enteramente ficticio: Servicio Empresarial de Gestión Administrativa Agro.
Propósito informado: orientación inicial sobre alternativas de gestión administrativa de cobros y pagos para organizaciones agropecuarias.
Público descrito en esta ficha simulada: asociaciones de productores legalmente constituidas.
Puede proponerse una reunión de orientación de 45 minutos, pero su disponibilidad debe confirmarse con el equipo comercial.
La evaluación de cualquier solicitud dependería de una revisión interna posterior.
No se proporcionan tarifas, tasas, comisiones, requisitos documentales específicos, condiciones contractuales, plazos, elegibilidad individual ni disponibilidad definitiva. No hay decisión de aprobación o contratación.

Organiza exactamente seis preguntas frecuentes en una tabla de tres columnas: pregunta, respuesta que permite la ficha, dato pendiente o límite. Incluye preguntas sobre propósito, destinatarios, reunión, requisitos documentales, tarifas/comisiones y revisión de una solicitud.

Para los datos no incluidos escribe "No disponible en la ficha ficticia; requiere validación institucional". No cites fuentes externas, no atribuyas funcionalidades reales al banco y no supongas acceso a sus sistemas.
```

**Paso 3.** Confirmar que las seis respuestas reflejan la ficha: propósito, público y posibilidad de reunión pueden describirse **solo en el escenario simulado**; precios, requisitos y decisiones no pueden presentarse como confirmados.

**Paso 4.** Si aparecen respuestas inventadas, enviar el siguiente ajuste.

**Prompt 4 — Corregir preguntas frecuentes sin respaldo**

```text
Revisa las seis preguntas frecuentes y conserva solo la información expresada en FICHA-VV-03. Si falta una tarifa, requisito, plazo o decisión, usa exactamente la frase "No disponible en la ficha ficticia; requiere validación institucional". No conviertas los datos simulados en información real de Banco Agrícola. Mantén seis preguntas y las tres columnas.
```

### Tarea 3. Identificar afirmaciones sin respaldo y ajustar el borrador (7 minutos)

**Paso 1.** Comparar la propuesta con los hechos de `FICHA-VV-03` y las seis preguntas frecuentes. Identificar qué afirmaciones están respaldadas **por la ficha simulada**, cuáles están ausentes y cuáles se han presentado con una seguridad injustificada.

**Paso 2.** Volver al **Generador de solicitudes de propuesta** y solicitar una versión corregida mediante este prompt.

**Prompt 5 — Revisión comercial final**

```text
Revisa el borrador de FICHA-VV-03 que redactaste. Compáralo únicamente con la ficha ficticia original de esta conversación. Señala brevemente cualquier afirmación sin respaldo sobre disponibilidad, precio, requisitos, tasas, plazos, aprobación, integraciones o compromisos.

Después entrega la versión corregida completa del borrador. Mantén el contexto de la asociación y el propósito del servicio ficticio. Propón la reunión de orientación de 45 minutos solo como posibilidad sujeta a confirmación. Al final, agrega una lista separada "Puntos por validar". No inventes datos ni presentes este ejercicio como oferta institucional real.
```

**Paso 3.** Verificar manualmente que la lista de puntos por validar incluya, cuando corresponda, disponibilidad de la reunión, requisitos documentales, tarifas o comisiones, condiciones contractuales y plazos. Comprobar que el borrador no garantiza contratación, aprobación ni elegibilidad.

**Paso 4.** Conservar como entregable la propuesta corregida junto con los puntos por validar y las preguntas frecuentes. No compartirlos como oferta comercial real.

### Resultado esperado

Existe un **borrador de propuesta** sobre el servicio **ficticio**, basado exclusivamente en `FICHA-VV-03`, y una **lista explícita de datos pendientes de validación**. Adicionalmente, se dispone de seis preguntas frecuentes coherentes con la ficha. Ningún texto confirma tasas, requisitos, servicios reales, resultados de evaluación o compromisos que no están sustentados.

[Volver a la lista de prácticas](../README.md)
