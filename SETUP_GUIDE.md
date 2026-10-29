# Setup Guide General

## Taller práctico de productividad con Microsoft Copilot y agentes de IA

| Control documental | Información |
|---|---|
| Repositorio | [Netec-Mx/TPRACT-AI-3025-LD-BA-MSV-Priv](https://github.com/Netec-Mx/TPRACT-AI-3025-LD-BA-MSV-Priv) |
| Rama y revisión analizada | `main` — `856163a67d1fdf7a4012ac5ccf9799acdb7d4cd8` |
| Cobertura documental | README principal, SETUP_GUIDE.md, los cinco README de capítulos, cinco prácticas, CODEOWNERS e inventario de recursos |
| Fecha de revisión | 29 de octubre de 2026 |
| Versión de esta guía | 1.0 |
| Modalidad | Navegador, servicios Microsoft 365 y documentos locales o en almacenamiento corporativo autorizado |

# Objetivo

Preparar un entorno común para todo el repositorio: acceso corporativo a Microsoft Copilot Chat, disponibilidad de los diez agentes indicados, un editor compatible con DOCX y una única estructura de almacenamiento con permisos de escritura.

La preparación termina cuando cada cuenta puede conversar con los agentes autorizados, editar y volver a abrir documentos, y conservarlos en las carpetas comunes. Esta guía contiene prerrequisitos, configuración y validación; no desarrolla las actividades del taller.

El repositorio distribuye documentación y un logotipo. No contiene instaladores, código de aplicaciones, paquetes de agentes, archivos de configuración ejecutables ni plantillas DOCX descargables. Las fuentes ficticias están incorporadas en los README. Su disponibilidad en GitHub no acredita que los agentes estén desplegados en el tenant del cliente.

# Requisitos de Hardware

| Recurso | Requisito consolidado del repositorio |
|---|---|
| Equipo | Computadora con procesador de 64 bits y dos núcleos o superior |
| Memoria | 8 GB de RAM como mínimo |
| Almacenamiento | 2 GB libres para documentos y archivos de trabajo |
| Pantalla | Mínimo 1366 × 768; recomendado 1920 × 1080 |
| Conectividad | Mínimo 10 Mbps de descarga y 2 Mbps de carga, con conexión estable durante toda la sesión |

Estos valores corresponden al puesto de trabajo descrito por las guías, no a requisitos de procesamiento local de un modelo de IA. No se necesita GPU, cámara, micrófono ni hardware de virtualización para las funciones documentadas.

# Sistemas Operativos Compatibles

El repositorio no establece una versión de sistema operativo. Sus comandos de preparación utilizan PowerShell y sus actividades se realizan en el navegador.

| Plataforma | Condición de uso |
|---|---|
| Windows | Base principal de preparación por los comandos PowerShell del repositorio. Utilizar una edición con soporte vigente y un navegador compatible actualizado. |
| macOS | Alternativa para la modalidad web, si el navegador, el editor y las políticas de acceso corporativo funcionan. Se incluyen comandos de carpetas equivalentes. |
| Linux | Alternativa condicionada a la validación de la modalidad web y al editor autorizado. No hay una distribución Linux ni compatibilidad de aplicaciones de escritorio certificadas por el repositorio. |

Las alternativas de macOS y Linux se deducen de la modalidad web; no constituyen evidencia de pruebas realizadas por el autor de los laboratorios. Validar el flujo completo en la plataforma elegida antes de asignarla al grupo. No se requiere instalar Office de escritorio para seguir la ruta con Word para la Web.

# Software Requerido

| Componente | Edición o versión | Preparación necesaria |
|---|---|---|
| Navegador | Microsoft Edge, Google Chrome, Mozilla Firefox o Apple Safari, en versión vigente compatible | JavaScript, inicio de sesión, copiado/pegado y descargas operativos. Registrar versión desde la opción Acerca de del navegador. |
| Microsoft Copilot Chat | Acceso corporativo; el repositorio lo denomina «Básico» | Cuenta Microsoft Entra ID con suscripción base elegible y servicio permitido por el tenant. |
| Agentes del taller | Diez agentes preexistentes administrados por el cliente | Acceso asignado a cada participante y conversación funcional. Ver inventario siguiente. |
| Editor de documentos | Word para la Web o aplicación equivalente autorizada compatible con DOCX | Crear y editar documentos, tablas, comentarios o resaltados; guardar, descargar cuando proceda y reabrir. |
| PowerShell | Versión disponible y autorizada en Windows; el repositorio no fija una versión | Crear carpetas y ejecutar diagnósticos. Los comandos de archivos no requieren módulos adicionales. |
| Almacenamiento | Carpeta local o ubicación corporativa autorizada | Lectura y escritura; OneDrive solo si se elige esa modalidad. |

Copilot Chat, Word para la Web y los agentes son servicios administrados: no se instala ni se fija una versión semántica local. Los marcadores `[VERSIÓN POR VALIDAR]` de los README se sustituyen por el registro de edición visible, fecha de acceso y configuración efectivamente disponible. No deben convertirse en números de versión inventados.

No se necesitan Python, .NET, Java, Node.js, SDK, IDE, Git, Azure CLI, PowerShell Microsoft Graph ni herramientas de desarrollo. Tampoco se requiere instalar una aplicación de escritorio de Copilot.

# Herramientas y Dependencias

## Inventario único de agentes

El cliente debe proporcionar el acceso o enlace interno de cada agente y comprobarlo con una cuenta equivalente a la del participante. Los nombres siguientes se conservan como aparecen en la documentación.

| Agente requerido | Dependencia de preparación |
|---|---|
| Asistente de indicaciones | Visible, accesible y capaz de responder a una solicitud de texto |
| Asistente de escritura | Visible, accesible y capaz de responder a una solicitud de texto |
| Diseñador de comunicaciones corporativas | Visible, accesible y capaz de responder a una solicitud de texto |
| Traductor de texto | Visible, accesible y capaz de responder a una solicitud de texto |
| Generador de solicitudes de propuesta | Visible, accesible y capaz de responder a una solicitud de texto |
| Asistente de información disponible | Visible, accesible y utilizable sin conexión a sistemas bancarios |
| Asesor de reuniones | Visible y utilizable con texto de minuta pegado en la conversación |
| Asistente de scrum | Visible y utilizable para producir texto o tablas, sin crear planes externos |
| Asistente de aprendizaje | Visible, accesible y capaz de responder a una solicitud de texto |
| Tutor de cuestionarios | Visible, accesible y capaz de responder a una solicitud de texto |

**Los nombres no acreditan identidad ni disponibilidad universal.** El repositorio describe agentes del entorno del cliente, pero no incluye identificadores, manifiestos, enlaces internos ni instrucciones para desplegarlos. No es posible afirmar que sean agentes estándar de Microsoft, asignarles un enlace público específico ni equipararlos automáticamente con otros asistentes de nombre parecido. Un vínculo genérico a Microsoft Learn tampoco identifica el agente correcto.

Antes del taller, el responsable del tenant debe dejar identificado para cada agente: nombre visible, enlace o identificador de acceso si está disponible, propietario/editor, grupo autorizado y modalidad de licencia o consumo. El registro no debe contener secretos. Si un agente no existe, el entorno aún no está completo para la ruta original.

## Licencias, cuentas y permisos

- Una cuenta de trabajo o laboratorio Microsoft Entra ID por participante, proporcionada por el cliente y habilitada para Copilot Chat mediante una suscripción elegible.
- Acceso de usuario a los diez agentes; no se requieren roles administrativos para participar.
- Derecho de uso del editor seleccionado. El acceso a Copilot Chat no garantiza por sí solo todos los servicios de edición o almacenamiento elegidos.
- Permiso para crear y modificar archivos en la ubicación común seleccionada.
- Método de autenticación multifactor y dispositivo conforme, cuando lo exijan las políticas existentes del cliente.

El complemento de pago de Microsoft 365 Copilot no es un requisito general de la ruta documentada. Sin embargo, **no debe asumirse que cualquier agente carece de costo adicional**: Microsoft distingue agentes basados en instrucciones o sitios públicos de agentes que utilizan datos compartidos del tenant y consumo medido. Como el repositorio no describe la implementación de sus diez agentes, el administrador debe verificar sus condiciones reales antes del curso.

No habilitar facturación por consumo, conectores ni acceso a datos corporativos para resolver una ausencia de agentes. El alcance documentado utiliza texto ficticio proporcionado en la conversación. Si una implementación existente exige capacidad adicional, el cliente debe resolver su disponibilidad previamente o autorizar una alternativa equivalente.

No se requieren licencias de Microsoft Designer, Planner, Teams, To Do ni funciones de Copilot dentro de Word. Las menciones a reuniones, tableros, comunicaciones y cuestionarios corresponden a generación de texto y documentos, sin reuniones reales ni publicación de tareas.

# Instalación y Configuración

## 1. Preparar el navegador y el acceso corporativo

1. Actualizar el navegador mediante el mecanismo autorizado del equipo.
2. Utilizar un perfil de navegador identificado con la cuenta del laboratorio y evitar mezclar sesiones personales y corporativas.
3. Abrir [Microsoft Copilot Chat](https://copilot.cloud.microsoft/). Si el tenant mantiene un acceso corporativo en [m365.cloud.microsoft](https://m365.cloud.microsoft/), usar el acceso publicado por TI y permitir su redirección oficial.
4. Iniciar sesión con la cuenta Microsoft Entra ID asignada y completar el método de autenticación requerido.
5. Confirmar en el perfil que la cuenta y organización corresponden al laboratorio. Registrar la etiqueta de acceso visible; no inferir la licencia a partir del nombre de la aplicación.
6. Probar una conversación breve sin información sensible y comprobar que el cuadro de entrada, la respuesta y el copiado del resultado funcionan.

El cambio de URL del servicio no convierte la experiencia en el Copilot de consumo para cuentas personales. Utilizar siempre el contexto corporativo autorizado.

## 2. Confirmar la disponibilidad de agentes

Abrir cada agente desde la lista o vínculo que entregue el cliente. Comprobar que el nombre y propietario corresponden al inventario autorizado y enviar un mensaje de prueba inocuo, por ejemplo: «Responde con un saludo breve de prueba, sin consultar ni modificar recursos externos».

Resultado esperado: los diez agentes permiten iniciar una conversación y devolver texto con la cuenta del participante. Que un agente aparezca en una lista no acredita que se pueda utilizar.

Los participantes no deben crear, instalar, modificar ni conceder permisos a agentes durante el setup. Si falta uno, registrar el nombre y el error y solicitar su revisión al responsable del entorno. Una sustitución por Copilot Chat debe quedar autorizada por el cliente/instructor y documentada como alternativa; no acredita la disponibilidad del agente original.

## 3. Habilitar edición y guardado

Abrir Word para la Web desde el iniciador de aplicaciones de la cuenta corporativa, o el editor equivalente autorizado. Comprobar creación de DOCX, inserción de tablas, comentarios o resaltado, y guardado.

Si se utiliza Word para la Web, verificar además su ubicación de almacenamiento corporativo y la descarga de una copia DOCX a la carpeta del taller cuando ese sea el flujo elegido. Este servicio guarda en almacenamiento cloud: una carpeta local por sí sola no habilita Word para la Web.

Si solo se dispone de un editor local autorizado, confirmar que conserva correctamente DOCX, tablas y anotaciones. No basta con un editor de texto plano para cumplir el formato de documento utilizado en todo el repositorio. No crear documentos «vacíos» con `New-Item` y extensión `.docx`: crear un documento válido desde el editor.

## 4. Unificar la ubicación de trabajo

Las guías alternan `<RUTA_BASE>`, `$HOME\OneDrive` y `$HOME`. Preparar **una sola ubicación** y utilizarla en todas las sesiones. La ruta lógica `/Copilot-Labs-BancoAgricola-Simulado/` de las guías representa la carpeta del taller; no obliga a escribir en la raíz del disco.

La configuración base siguiente usa almacenamiento local bajo el perfil del usuario. Si TI elige una carpeta sincronizada, establecer su ruta real una sola vez antes de crear las subcarpetas. No asumir que OneDrive se llama exactamente `OneDrive` ni que está aprovisionado en todos los equipos.

### Windows PowerShell

```powershell
$labRoot = Join-Path $env:USERPROFILE 'Copilot-Labs-BancoAgricola-Simulado'
$folders = @(
    '01-Prompts',
    '02-Comunicaciones',
    '03-Propuestas',
    '04-Reuniones',
    '05-Aprendizaje'
)

New-Item -ItemType Directory -Force -Path $labRoot | Out-Null
foreach ($folder in $folders) {
    New-Item -ItemType Directory -Force -Path (Join-Path $labRoot $folder) | Out-Null
}

(Resolve-Path -LiteralPath $labRoot).Path
Get-ChildItem -LiteralPath $labRoot -Directory | Select-Object Name
```

Resultado esperado: una ruta absoluta como `C:\Users\usuario\Copilot-Labs-BancoAgricola-Simulado` y las cinco subcarpetas. Ejecutar nuevamente estos comandos conserva los archivos existentes.

### macOS o Linux, si se aprueba la modalidad web

```bash
lab_root="$HOME/Copilot-Labs-BancoAgricola-Simulado"
mkdir -p "$lab_root/01-Prompts" "$lab_root/02-Comunicaciones" \
  "$lab_root/03-Propuestas" "$lab_root/04-Reuniones" \
  "$lab_root/05-Aprendizaje"
cd "$lab_root"
pwd
ls -d */
```

Resultado esperado: ruta absoluta bajo el directorio personal y las mismas cinco subcarpetas. No es necesario instalar PowerShell en estas plataformas.

# Configuración Base para los Laboratorios

## Almacenamiento y nombres de archivo

Conservar esta estructura durante todo el taller:

```text
Copilot-Labs-BancoAgricola-Simulado/
├── 01-Prompts/
├── 02-Comunicaciones/
├── 03-Propuestas/
├── 04-Reuniones/
└── 05-Aprendizaje/
```

Usar la nomenclatura común `LAB##_INICIALES_Descripcion_v##.docx`, reemplazando el número, las iniciales y la descripción cuando corresponda. Conservar versiones iniciales y revisadas. El setup crea carpetas y verifica el editor; no necesita generar de antemano los entregables de las prácticas.

En todos los comandos posteriores del material original, asignar `$labRoot` a la ubicación absoluta elegida. Evitar que un bloque vuelva a cambiarla a otra carpeta. Las variables de PowerShell no distinguen mayúsculas de minúsculas: `$LabRoot` y `$labRoot` representan la misma variable.

## Fuentes y plantillas

Mantener accesible la documentación completa, especialmente los escenarios, la ficha ficticia de condiciones, la minuta ficticia y la guía institucional ficticia incluidos en los README. No se requieren descargas de datos reales ni acceso a sistemas bancarios.

Las guías mencionan plantillas del instructor para propuestas, inducción y cuestionarios, pero el repositorio no las distribuye como archivos. Antes de la sesión, confirmar que esas plantillas estarán disponibles o dejar acordado el uso de documentos nuevos con las estructuras del propio material. Una plantilla opcional de propuesta no debe bloquear la preparación si no se entrega.

Utilizar únicamente las fuentes ficticias del material o las equivalentes autorizadas por el instructor. Las direcciones con dominio `.example` que aparecen en los casos son datos de muestra; no son servicios que deban resolverse, configurarse o probarse mediante correo.

## Configuraciones locales

No se requieren `.env`, variables de entorno persistentes, claves de API, tokens, cadenas de conexión ni archivos JSON de configuración. `$labRoot`, `$folders` y `lab_root` son variables temporales de los comandos de preparación. No modificar `HOME`, `USERPROFILE` ni `PATH`.

No se necesitan bases de datos, servidores locales, puertos entrantes, contenedores, máquinas virtuales, simuladores ni emuladores. Tampoco se requiere una suscripción Azure o AWS del participante.

# Servicios Externos Requeridos

| Servicio | Uso necesario |
|---|---|
| Microsoft Entra ID | Inicio de sesión de la cuenta corporativa o de laboratorio |
| Microsoft Copilot Chat y agentes del tenant | Conversación y generación de texto |
| Microsoft 365 de edición y almacenamiento | Solo los servicios utilizados para Word para la Web y el guardado cloud elegido |
| GitHub | Consulta o descarga de las guías; no se requiere una cuenta de GitHub para leer el repositorio público |

TI debe permitir los endpoints vigentes de Microsoft 365 y Copilot según la [documentación oficial de requisitos de red](https://learn.microsoft.com/en-us/microsoft-365/copilot/microsoft-copilot-requirements), incluida la transición a `copilot.cloud.microsoft` y el dominio `*.cloud.microsoft`. La lista de tres hosts de los diagnósticos siguientes es orientativa y **no sustituye la lista completa de endpoints**.

Mantener HTTPS saliente, resolución DNS y los mecanismos de autenticación del tenant operativos. Permitir cookies y almacenamiento de sesión necesarios mediante la configuración institucional. Si Safe Links impide abrir enlaces, revisar con TI la excepción específica documentada para `safelinks.protection.outlook.com`; no desactivar globalmente las protecciones del navegador.

No se requieren buzón de correo, calendario, reuniones de Teams ni conectores bancarios para las tareas documentadas. Una dependencia de almacenamiento o autenticación impuesta por el servicio realmente elegido debe quedar resuelta antes del taller.

# Validación del Entorno

La aprobación requiere verificación en la sesión autenticada de cada participante. Los diagnósticos de terminal complementan esta revisión, pero no demuestran licenciamiento ni acceso a agentes.

| Control | Resultado esperado |
|---|---|
| Cuenta | Cuenta Microsoft Entra ID asignada, organización correcta y autenticación completada |
| Chat | Conversación nueva responde y permite copiar texto |
| Agentes | 10 de 10 identificados, accesibles y con respuesta de prueba satisfactoria |
| Navegador | Versión registrada, sesiones y descargas funcionales |
| Editor | Documento DOCX válido con texto, tabla y anotación que se guarda y vuelve a abrir |
| Carpetas | Las cinco subcarpetas existen en una sola raíz absoluta |
| Permisos | Se puede crear, leer y eliminar un archivo temporal propio |
| Materiales | Guías completas y fuentes ficticias accesibles; plantillas o su modalidad de reemplazo resueltas |
| Licencias | Suscripción base y editor confirmados; condiciones de los agentes revisadas por el cliente |

Para validar el editor, crear desde la aplicación un documento temporal de setup con un texto breve, una tabla de dos columnas y un comentario o resaltado. Guardarlo como DOCX en la ubicación autorizada, cerrarlo y volverlo a abrir. Comprobar que conserva los tres elementos. Esta verificación no exige Copilot integrado en Word.

Registrar fecha, sistema operativo, navegador y versión, raíz absoluta, etiqueta de Copilot y resultado de acceso a agentes. No incluir contraseñas, códigos MFA, tokens, cookies ni capturas con información confidencial.

# Comandos de Verificación

## Windows PowerShell: equipo y conectividad

```powershell
$PSVersionTable.PSVersion
Get-CimInstance Win32_OperatingSystem |
    Select-Object Caption, Version, OSArchitecture
Get-CimInstance Win32_ComputerSystem |
    Select-Object NumberOfLogicalProcessors,
        @{Name='RAM_GB';Expression={[math]::Round($_.TotalPhysicalMemory / 1GB, 1)}}
Get-CimInstance Win32_Processor |
    Select-Object Name, NumberOfCores, AddressWidth
Get-PSDrive -PSProvider FileSystem |
    Select-Object Name, Root, @{Name='Libre_GB';Expression={[math]::Round($_.Free / 1GB, 1)}}
```

Resultado esperado: sistema y CPU de 64 bits, al menos dos núcleos, 8 GB de RAM y 2 GB disponibles en la unidad elegida. En equipos que reservan memoria al hardware, contrastar el valor informado con la RAM física instalada.

```powershell
$serviceHosts = @(
    'copilot.cloud.microsoft',
    'login.microsoftonline.com',
    'github.com'
)
foreach ($serviceHost in $serviceHosts) {
    Resolve-DnsName -Name $serviceHost -ErrorAction Continue
    Test-NetConnection -ComputerName $serviceHost -Port 443 -InformationLevel Detailed
}
```

Resultado esperado: DNS devuelve registros y `TcpTestSucceeded` es `True` cuando hay salida directa permitida. En redes que obligan a usar un proxy, la prueba TCP directa puede fallar aunque el navegador funcione; TI debe comprobar el recorrido autorizado mediante proxy.

## Windows PowerShell: estructura y permisos

Ejecutar con `$labRoot` y `$folders` definidos como en la preparación:

```powershell
foreach ($folder in $folders) {
    $path = Join-Path $labRoot $folder
    [pscustomobject]@{
        Carpeta = $folder
        Existe = Test-Path -LiteralPath $path -PathType Container
    }
}

$testFile = Join-Path $labRoot ('setup-' + [guid]::NewGuid().ToString() + '.tmp')
try {
    Set-Content -LiteralPath $testFile -Value 'SETUP_OK' -Encoding UTF8 -ErrorAction Stop
    Get-Content -LiteralPath $testFile -ErrorAction Stop
}
finally {
    if (Test-Path -LiteralPath $testFile) {
        Remove-Item -LiteralPath $testFile -ErrorAction Stop
    }
}
```

Resultado esperado: `True` en las cinco filas y lectura de `SETUP_OK`. Solo se elimina el archivo temporal recién creado.

## macOS o Linux: diagnóstico equivalente

```bash
uname -sm
curl --version
curl -L -sS -o /dev/null -w 'HTTP final: %{http_code}\n' \
  --connect-timeout 10 --max-time 30 https://copilot.cloud.microsoft/

for folder in 01-Prompts 02-Comunicaciones 03-Propuestas 04-Reuniones 05-Aprendizaje; do
  if [ -d "$lab_root/$folder" ]; then
    printf '%s: OK\n' "$folder"
  else
    printf '%s: FALTA\n' "$folder"
  fi
done

test_file=$(mktemp "$lab_root/setup-XXXXXX") && {
  printf 'SETUP_OK\n' > "$test_file" && cat "$test_file"
  rm -f -- "$test_file"
}
```

Resultado esperado: arquitectura de 64 bits, cinco carpetas con `OK` y lectura de `SETUP_OK`. La consulta HTTP utiliza el cliente cURL si está disponible en la estación; no es una dependencia de ejecución del taller. Un código `000` indica que no se obtuvo respuesta HTTP y requiere revisar la conexión o TLS. Una página pública o de autenticación puede responder sin que la cuenta tenga acceso al chat: comprobar siempre la sesión en el navegador.

## Comprobaciones que requieren navegador

No hay una CLI de Copilot Chat ni un wrapper del repositorio que valide los diez agentes con las credenciales del participante. No sustituir esta prueba por `ping`, por un `HTTP 200` o por la simple existencia de una licencia.

Completar la tabla de validación dentro del navegador, usando la cuenta asignada. No es necesario instalar módulos administrativos, registrar aplicaciones Entra ni automatizar el inicio de sesión para preparar este taller.

# Troubleshooting

| Síntoma | Comprobación y corrección |
|---|---|
| El navegador muestra una experiencia personal | Revisar la cuenta activa y abrir el acceso corporativo publicado por TI. Utilizar un perfil separado para el laboratorio. |
| Copilot Chat no está disponible | Comprobar suscripción base elegible, habilitación de la cuenta y restricciones del tenant. No asumir que basta con crear un usuario Entra. |
| Un agente no aparece o devuelve acceso denegado | Confirmar identidad del agente, grupo de acceso, cuenta utilizada y condición de licencia/consumo. Registrar nombre, hora y mensaje de error. El cliente debe resolver el acceso antes del taller o autorizar una alternativa. |
| Se propone instalar un agente de nombre similar | Contrastar propietario e identificador con el inventario del cliente. El repositorio no proporciona un catálogo público verificable de sus agentes. |
| El agente pide consentimiento, conectores o capacidad de pago | No concederlos durante la sesión. Revisar la implementación con el responsable del tenant y mantener el alcance de texto ficticio sin integraciones externas. |
| Una URL cambia o redirige | Usar la URL corporativa vigente y permitir las redirecciones oficiales a `copilot.cloud.microsoft`. Revisar proxy y filtrado con TI. |
| DNS o HTTPS fallan | Revisar red, proxy institucional, certificados y endpoints permitidos. No desactivar TLS ni controles corporativos como solución. |
| No se abren enlaces de una respuesta | Revisar políticas de cookies y Safe Links con TI; aplicar únicamente las excepciones necesarias documentadas por Microsoft. |
| Los archivos se guardan en ubicaciones distintas | Unificar `$labRoot` en los bloques originales y verificar su ruta absoluta. No mezclar `$HOME`, una carpeta OneDrive supuesta y otra raíz local. |
| Word para la Web no guarda en la carpeta local | Confirmar guardado cloud y descargar una copia DOCX a la raíz autorizada, o utilizar el editor local autorizado. Probar el flujo completo antes de iniciar. |
| Un DOCX no se puede abrir | Crear documentos válidos desde Word o el editor compatible. Un archivo de texto con extensión `.docx` no es un documento Word. |
| Faltan fuentes o plantillas | Consultar las fuentes incorporadas en los README y confirmar las plantillas del instructor o la estructura documental acordada. No reemplazarlas con documentación bancaria real. |
| El chat presenta límites o indisponibilidad temporal | Volver a comprobar en una conversación de prueba y comunicar el estado al instructor. No resolverlo cambiando a una cuenta personal o comprando licencias durante la sesión. |

# Checklist Final

- [ ] Equipo con 64 bits, dos núcleos, 8 GB de RAM y 2 GB libres.
- [ ] Conexión estable de al menos 10 Mbps de descarga y 2 Mbps de carga.
- [ ] Navegador actualizado, con sesión corporativa, copiado y descargas comprobados.
- [ ] Cuenta Microsoft Entra ID y suscripción base elegible confirmadas.
- [ ] Autenticación y políticas de acceso del cliente satisfechas.
- [ ] Copilot Chat responde con la cuenta asignada.
- [ ] Los diez agentes están identificados, disponibles y probados; cualquier alternativa está documentada.
- [ ] Licencias y condiciones de consumo de los agentes resueltas antes de la sesión.
- [ ] Editor compatible con DOCX, tablas y anotaciones validado mediante guardado y reapertura.
- [ ] Una única raíz absoluta con las cinco subcarpetas y permisos de escritura.
- [ ] Guías y fuentes ficticias accesibles; plantillas o modalidad equivalente preparadas.
- [ ] Registro de validación completado sin secretos ni información de clientes reales.

# Resumen

El entorno común es una estación con navegador, cuenta corporativa, Copilot Chat, los diez agentes habilitados por el cliente y un editor DOCX con almacenamiento autorizado. La preparación no exige infraestructura de desarrollo ni servicios bancarios.

La disponibilidad del chat no acredita la de los agentes. La condición decisiva para aprobar el entorno es comprobar acceso y respuesta con las cuentas reales del taller, junto con la edición y persistencia de documentos en una sola ubicación.

## Correcciones consolidadas aplicadas

| Hallazgo del repositorio | Criterio de esta guía |
|---|---|
| SETUP_GUIDE.md apunta a `Netec-Mx/261028-TPRACT-AI-3025-LD-BA-MSV-Priv` | Se utiliza el repositorio real sin el prefijo de fecha. |
| Versiones SaaS y fuentes de agentes quedan como marcadores | Se registra edición/fecha/configuración; los agentes se identifican con información del tenant. No se inventan versiones ni enlaces. |
| «Básico» aparece junto con agentes no identificados | Se exige validar el acceso efectivo y la condición de uso de cada agente. No se garantiza inclusión universal. |
| Rutas alternan una base variable, OneDrive y el perfil personal | Se prepara una raíz única y se reutiliza en todos los comandos. |
| Word o un editor equivalente se explicita solo en algunos capítulos | Se consolida como dependencia común por el uso de DOCX, tablas y revisión documental. |
| Plantillas del instructor no están distribuidas | Se identifica la dependencia y se prepara su entrega o la estructura equivalente antes del taller. |
| Referencias a Teams, Planner, To Do o Microsoft 365 Copilot | No se añaden como instalaciones ni licencias obligatorias porque la ejecución documentada no las utiliza. |

## Alcance de la validación de esta guía

Se inspeccionó la totalidad del contenido documental de los cinco capítulos y los archivos generales del commit indicado. Se contrastaron requisitos de acceso, agentes, navegador y red con documentación oficial de Microsoft. La presencia de un logotipo y CODEOWNERS se verificó en el inventario; no agregan dependencias de ejecución.

No se dispuso del tenant, cuentas ni agentes del cliente. Por ello, no se afirma haber probado su disponibilidad, sus licencias ni el guardado en Microsoft 365. Los comandos PowerShell y la experiencia autenticada deben ejecutarse en la estación de destino; la guía distingue estas comprobaciones de la revisión documental completada.

## Fuentes

- [Repositorio completo en la revisión analizada](https://github.com/Netec-Mx/TPRACT-AI-3025-LD-BA-MSV-Priv/tree/856163a67d1fdf7a4012ac5ccf9799acdb7d4cd8).
- [Microsoft: requisitos de Copilot, navegador, identidad y red](https://learn.microsoft.com/en-us/microsoft-365/copilot/microsoft-copilot-requirements).
- [Microsoft: compra y administración de agentes en Copilot Chat](https://learn.microsoft.com/en-us/copilot/manage-agents-copilot-chat).
- [Microsoft: diferencias de acceso a Copilot Chat con y sin licencia adicional](https://support.microsoft.com/es-es/microsoft-365-copilot/how-copilot-chat-works-with-and-without-a-microsoft-365-copilot-license).
- [Microsoft: ayuda de Word](https://support.microsoft.com/es-es/word).
- [PowerShell: New-Item](https://learn.microsoft.com/en-us/powershell/module/microsoft.powershell.management/new-item).
- [PowerShell: Test-NetConnection](https://learn.microsoft.com/en-us/powershell/module/nettcpip/test-netconnection).
- [PowerShell: Resolve-DnsName](https://learn.microsoft.com/en-us/powershell/module/dnsclient/resolve-dnsname).
- [cURL: documentación oficial de opciones](https://curl.se/docs/manpage.html).
