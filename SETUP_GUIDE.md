# Setup Guide General

## Taller práctico de productividad con Microsoft Copilot y agentes de IA

## Descripción del entorno

Las cinco prácticas se realizan en **Microsoft Copilot Chat Básico**, desde un navegador y con los agentes previstos en el temario, **previamente disponibles para cada participante**. Las fichas ficticias, los prompts y los textos fuente están incorporados en los `README.md` de cada capítulo. No se requieren conexiones a sistemas bancarios, listas de clientes, bases de datos, grabaciones de reuniones ni archivos externos para ejecutar las actividades.

Este documento prepara el acceso y los materiales; no sustituye las prácticas.

## Requisitos de hardware y software

| Recurso | Requisito |
| --- | --- |
| Equipo | Computadora de uso personal o corporativo con teclado y acceso a Internet estable |
| Navegador | Microsoft Edge, Chrome u otro navegador vigente compatible con Microsoft 365 según TI |
| Aplicación | [Microsoft Copilot Chat](https://m365.cloud.microsoft/chat) en la sesión institucional |
| Documentación | Los cinco `README.md` accesibles desde GitHub o GitHub Pages |
| Editor de texto o documentos | **Opcional**: Word, Bloc de notas u otra herramienta autorizada si se decide guardar los borradores. No es necesaria una licencia Copilot en Word |

No es necesario instalar PowerShell, SDK, IDE, Python, Node.js, extensiones, máquinas virtuales ni herramientas de integración.

## Cuentas, licencias y permisos

Disponer de una cuenta laboral o educativa de Microsoft Entra ID con una suscripción elegible y acceso a Copilot Chat Básico, habilitado conforme a las políticas del cliente. Comprobar que se pueden abrir y utilizar los agentes indicados en el taller; la sola presencia del nombre de una plantilla no garantiza su disponibilidad.

| Denominación del temario | Referencia funcional o de plantilla Microsoft, cuando existe | Práctica |
| --- | --- | --- |
| Asistente de indicaciones | `Prompt Coach` | 1 |
| Asistente de escritura | `Writing Coach` | 1 y 2 |
| Diseñador de comunicaciones corporativas | `Corporate Communications Crafter` | 2 |
| Traductor de texto | `Text Translator` | 2 |
| Generador de solicitudes de propuesta | `Request for Proposal Generator` | 3 |
| Asistente de información disponible | Nombre específico del cliente; equivalencia oficial no verificada | 3 |
| Asesor de reuniones | `Meeting Coach` | 4 |
| Asistente de scrum | `Scrum Assistant` | 4 |
| Asistente de aprendizaje | `Learning Coach` | 5 |
| Tutor de cuestionarios | `Quiz Tutor` | 5 |

**Aclaración esencial.** Varios de estos nombres aparecen en la documentación de Microsoft como **plantillas de Agent Builder**. Son puntos de partida para crear agentes, no agentes que existan automáticamente para todo usuario. El cliente debe confirmar qué agentes ha publicado o compartido, sus nombres reales y permisos, antes del taller. No se creará ni instalará un agente durante las prácticas. El **Asistente de información disponible** debe identificarse por su nombre o vínculo facilitado por el cliente; no se debe asumir una equivalencia oficial.

Los agentes basados en instrucciones y contenido público pueden estar incluidos en Copilot Chat Básico; agentes que consulten datos compartidos de la organización pueden requerir **configuración administrativa, una licencia apropiada o facturación por consumo**. No activar facturación por uso ni conectar datos corporativos como parte del taller. El cliente debe confirmar sus condiciones de acceso y costo.

## Preparación del entorno

**Paso 1.** Abrir [Copilot Chat](https://m365.cloud.microsoft/chat) e iniciar sesión con la cuenta **institucional** destinada a la capacitación. Confirmar la organización de la cuenta y completar la autenticación que solicite el tenant.

**Paso 2.** Abrir un chat nuevo y enviar una prueba inocua, como `Escribe una frase de bienvenida para un taller sobre productividad, sin usar datos externos`. Confirmar que devuelve texto y permite copiarlo.

**Paso 3.** Ubicar la sección **Agentes** o la ubicación equivalente de la interfaz. Abrir los diez agentes del inventario por los nombres habilitados por el cliente. Si el nombre no coincide, revisar el vínculo o denominación que haya proporcionado el responsable del taller; no tratar una **plantilla no desplegada** como un agente operativo.

**Paso 4.** Enviar a cada agente, cuando proceda, un mensaje de comprobación sin datos personales:

```text
Explica en una sola frase de qué manera puedes ayudarme con una actividad de capacitación. No consultes archivos, correos, bases de datos ni servicios externos. No modifiques recursos.
```

**Paso 5.** Mantener disponible la [lista de prácticas](README.md) y la guía del capítulo correspondiente. Verificar que se puede copiar y pegar texto entre conversaciones. Si se exige guardar productos, preparar una ubicación corporativa o local autorizada donde conservar los borradores.

**Paso 6.** Confirmar que las funciones de los agentes se utilizarán solo para **generar y revisar texto**; ningún capítulo requiere crear tareas reales en Planner, enviar correos, reservar reuniones, acceder a SharePoint ni consultar servicios financieros.

## Verificación del entorno

| Comprobación | Resultado aceptable |
| --- | --- |
| Cuenta | Inicio de sesión institucional correcto |
| Chat | Se puede enviar un mensaje, recibir una respuesta y copiarla |
| Agentes | Los diez agentes del temario, incluidos los compartidos por el cliente, responden con la cuenta del participante |
| Materiales | Están accesibles los `README.md` de los cinco capítulos |
| Transferencia de textos | Es posible copiar un resultado a una nueva conversación sin depender de memoria compartida entre agentes |
| Protección de datos | Las cuentas del taller no requieren introducir información personal o financiera real |

Si falta un agente, indicar al administrador o coordinador **qué agente no está disponible y qué error aparece**. La tarea correspondiente solo podrá ejecutarse como está diseñada cuando el acceso se resuelva. No sustituirlo silenciosamente por otro agente ni por un chat genérico, ya que eso alteraría la demostración solicitada.

## Seguridad y consideraciones adicionales

- Utilizar solo los nombres, casos, minutas, documentos y servicios **ficticios** de las guías. No copiar datos verdaderos de clientes, información bancaria confidencial, credenciales ni números de cuenta.
- Tratar las salidas de IA como borradores sujetos a **revisión humana**. Las condiciones, los documentos y los servicios de los ejemplos no son información oficial de Banco Agrícola.
- No enviar correos, crear registros reales, publicar propuestas, conectar fuentes externas ni comprometer operaciones de negocio.
- Las respuestas de un modelo generativo pueden variar. Comprobar los hechos, restricciones y resultados según las instrucciones de cada práctica.
- No se requiere una versión local concreta de Copilot Chat: es un servicio web que cambia con la configuración del cliente. La disponibilidad final de agentes y licencias debe comprobarse con una cuenta real del taller.

## Referencias oficiales

- [Microsoft Learn — Introducción a Copilot Chat](https://learn.microsoft.com/en-us/copilot/overview).
- [Microsoft Learn — Preguntas frecuentes de Copilot Chat](https://learn.microsoft.com/en-us/copilot/faq).
- [Microsoft Learn — Plantillas de Agent Builder](https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/agent-templates-overview).
- [Microsoft Learn — Licenciamiento y administración de agentes](https://learn.microsoft.com/en-us/copilot/agents).
- [Microsoft Learn — Protección de datos empresariales](https://learn.microsoft.com/en-us/microsoft-365/copilot/enterprise-data-protection).

Las referencias documentan las capacidades del producto; no prueban que los agentes específicos estén implementados en el tenant del cliente.