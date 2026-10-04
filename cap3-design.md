# Capítulo III: Solution UI/UX Design

## 3.1.1. Style Guidelines

### 3.1.1.1. General Style Guidelines

**1. Branding y Tono de Comunicación**

**2. Typography (Tipografía)**

**3. Colors (Paleta de Colores)**

**4. Spacing y Grid**

## 3.1.2. Information Architecture

### 3.1.2.1. Organization Systems

### 3.1.2.2. Labelling Systems

### 3.1.2.3. SEO Tags and Meta Tags

### 3.1.2.4. Searching Systems

### 3.1.2.5. Navigation Systems

## 3.1.3. Landing Page UI Design
### 3.1.3.1. Landing Page Wireframe
### 3.1.3.2. Landing Page Mock-up

## 3.1.4. Mobile Applications UX/UI Design
### 3.1.4.1. Mobile Applications Wireframes

Los siguientes wireframes presentan las principales vistas de la aplicación móvil Vantage PMO. Se organizan según el recorrido del usuario: acceso, registro, consulta del dashboard y gestión de proyectos, análisis, gobernanza y perfil. Las pantallas representan tanto vistas principales como estados de confirmación y formularios necesarios para comprender la navegación propuesta.

**Principios y elementos de diseño.** La propuesta prioriza la jerarquía visual y la consistencia entre pantallas: encabezados que identifican la sección, contenido agrupado por tarea, controles ubicados cerca de la información relacionada y acciones principales destacadas. Se aplican visibilidad del estado del sistema y retroalimentación mediante indicadores de avance, etiquetas de estado y confirmaciones; además, los pasos y opciones visibles favorecen el reconocimiento frente a la memorización. La interfaz usa una composición de una columna, tipografía jerarquizada, espacios de separación, superficies agrupadas, botones de acción y componentes de datos como métricas, filtros y barras de progreso.

**Diseño inclusivo.** La presentación móvil mantiene una lectura lineal y agrupa los formularios por propósito. Las etiquetas textuales acompañan a los iconos de navegación; los estados también se expresan con texto, números o indicadores, y no únicamente mediante color. El registro y la recuperación de contraseña muestran pasos consecutivos, mientras que los mensajes de éxito explican el resultado de las acciones. Estos wireframes establecen una intención de diseño inclusivo, pero no demuestran por sí solos conformidad: en la implementación se deberán validar contraste, ampliación del texto, áreas táctiles, navegación por teclado y nombres accesibles para tecnologías de asistencia, tomando WCAG 2.2 nivel AA como referencia.

**Arquitectura de información.** Antes de iniciar sesión, la información se organiza en acceso, recuperación de credenciales y creación de cuenta. Después de autenticarse, una navegación persistente agrupa las áreas principales en Home, Projects, Analytics, Governance y Profile. Dentro de cada área, la jerarquía conduce de la vista general a una tarea concreta por ejemplo, seleccionar un proyecto, revisar una alerta o editar la cuenta— y presenta confirmaciones al completar acciones relevantes. Esta organización responde a la necesidad identificada de consultar desde el móvil el estado de los proyectos, sus responsables, fechas, indicadores y alertas desde un punto centralizado.

#### 3.1.4.1.1. Authentication

El recorrido de autenticación comienza con la pantalla de inicio de Vantage PMO y el formulario de acceso. Si el usuario no recuerda sus credenciales, puede solicitar un código, verificarlo, definir una nueva contraseña y confirmar la actualización. La secuencia hace visible el paso actual y ofrece una confirmación final; la pantalla de cierre exitoso comunica que la sesión terminó.

| Inicio de la aplicación | Acceso | Recuperación por correo |
|:--:|:--:|:--:|
| <img src="assets/images/chapter-3/application-ux-ui-design/application-wireframes/authentication/mobile-splash-screen.png" alt="Pantalla de inicio de Vantage PMO" width="175"> | <img src="assets/images/chapter-3/application-ux-ui-design/application-wireframes/authentication/login-screen.png" alt="Formulario de inicio de sesión" width="175"> | <img src="assets/images/chapter-3/application-ux-ui-design/application-wireframes/authentication/password-recovery-email.png" alt="Solicitud de recuperación de contraseña por correo" width="175"> |

| Verificación del código | Nueva contraseña | Recuperación completada |
|:--:|:--:|:--:|
| <img src="assets/images/chapter-3/application-ux-ui-design/application-wireframes/authentication/password-recovery-verification-code.png" alt="Verificación del código de seguridad" width="175"> | <img src="assets/images/chapter-3/application-ux-ui-design/application-wireframes/authentication/password-recovery-new-password.png" alt="Formulario para crear una contraseña nueva" width="175"> | <img src="assets/images/chapter-3/application-ux-ui-design/application-wireframes/authentication/password-recovery-success.png" alt="Confirmación de contraseña actualizada" width="175"> |


#### 3.1.4.1.2. Registration

El registro se divide en cuatro pasos datos personales, contacto y acceso, perfil profesional y selección de rol seguidos por una pantalla de cuenta creada. El indicador numerado permite reconocer el avance y anticipar cuánto falta; la agrupación de campos reduce la carga de cada pantalla. La selección de rol introduce una arquitectura personalizada según las responsabilidades del usuario dentro de la PMO.

| Datos personales | Contacto y acceso | Perfil profesional |
|:--:|:--:|:--:|
| <img src="assets/images/chapter-3/application-ux-ui-design/application-wireframes/registration/registration-personal-information.png" alt="Primer paso del registro: datos personales" width="175"> | <img src="assets/images/chapter-3/application-ux-ui-design/application-wireframes/registration/registration-contact-and-access.png" alt="Segundo paso del registro: contacto y acceso" width="175"> | <img src="assets/images/chapter-3/application-ux-ui-design/application-wireframes/registration/registration-professional-profile.png" alt="Tercer paso del registro: perfil profesional" width="175"> |

| Selección de rol | Registro completado |
|:--:|:--:|
| <img src="assets/images/chapter-3/application-ux-ui-design/application-wireframes/registration/registration-role-selection.png" alt="Cuarto paso del registro: selección de rol" width="175"> | <img src="assets/images/chapter-3/application-ux-ui-design/application-wireframes/registration/registration-success.png" alt="Confirmación de cuenta creada" width="175"> |

#### 3.1.4.1.3. Dashboard

El dashboard es la entrada al espacio de trabajo autenticado. Presenta primero el saludo y el contexto del usuario, después una alerta prioritaria y métricas resumidas de proyectos, hitos, salud y capacidad. Esta jerarquía permite detectar asuntos que requieren atención antes de profundizar en cada proyecto. La barra inferior mantiene accesibles las cinco áreas principales y combina icono con etiqueta.

<p align="center"><img src="assets/images/chapter-3/application-ux-ui-design/application-wireframes/dashboard/home-dashboard.png" alt="Dashboard móvil con alerta prioritaria, métricas y navegación principal" width="220"></p>

#### 3.1.4.1.4. Projects

La sección de proyectos organiza el trabajo desde una lista filtrable hacia la creación de iniciativas, el tablero Kanban y acciones de seguimiento. Los formularios agrupan la identificación, los participantes y las fechas; el tablero permite consultar tareas por estado y equipo, mientras que la creación de una tarea muestra un formulario contextual y una confirmación. Las vistas de exportación y roadmap amplían el recorrido hacia la consulta ejecutiva y la planificación del portafolio.

| Lista de proyectos | Crear proyecto | Proyecto creado |
|:--:|:--:|:--:|
| <img src="assets/images/chapter-3/application-ux-ui-design/application-wireframes/projects/project-list.png" alt="Lista móvil de proyectos con filtros e indicadores" width="175"> | <img src="assets/images/chapter-3/application-ux-ui-design/application-wireframes/projects/project-creation-form.png" alt="Formulario de creación de proyecto" width="175"> | <img src="assets/images/chapter-3/application-ux-ui-design/application-wireframes/projects/project-creation-success.png" alt="Confirmación de proyecto creado" width="175"> |

| Confirmación con detalles | Crear tarea en Kanban | Tarea registrada |
|:--:|:--:|:--:|
|  <img src="assets/images/chapter-3/application-ux-ui-design/application-wireframes/projects/kanban-task-created-success.png" alt="Confirmación de tarea agregada al tablero Kanban" width="175">  | <img src="assets/images/chapter-3/application-ux-ui-design/application-wireframes/projects/kanban-task-creation-modal.png" alt="Formulario contextual para crear una tarea" width="175"> |<img src="assets/images/chapter-3/application-ux-ui-design/application-wireframes/projects/project-creation-success-details.png" alt="Confirmación detallada de iniciativa creada" width="175">|

| Exportar reporte | Dossier exportado | Roadmap estratégico |
|:--:|:--:|:--:|
| <img src="assets/images/chapter-3/application-ux-ui-design/application-wireframes/projects/project-report-export-modal.png" alt="Selección del formato y periodo de exportación del reporte" width="175"> | <img src="assets/images/chapter-3/application-ux-ui-design/application-wireframes/projects/project-dossier-export-success.png" alt="Confirmación de dossier de proyecto exportado" width="175"> | <img src="assets/images/chapter-3/application-ux-ui-design/application-wireframes/projects/strategic-roadmap.png" alt="Roadmap estratégico con hitos y trayectoria del portafolio" width="175"> |

#### 3.1.4.1.5. Analytics

Analytics presenta indicadores de eficiencia y desempeño en una vista resumida. Los filtros temporales permiten delimitar el análisis y la acción de exportación abre una selección de periodo y formato. La pantalla de éxito cierra ese flujo e informa que el reporte fue generado, haciendo visible el resultado de la acción.

| Dashboard analítico | Configurar exportación | Exportación completada |
|:--:|:--:|:--:|
| <img src="assets/images/chapter-3/application-ux-ui-design/application-wireframes/analytics/analytics-dashboard.png" alt="Dashboard de analítica con indicadores de desempeño" width="175"> | <img src="assets/images/chapter-3/application-ux-ui-design/application-wireframes/analytics/analytics-report-export-modal.png" alt="Modal para configurar la exportación del reporte analítico" width="175"> | <img src="assets/images/chapter-3/application-ux-ui-design/application-wireframes/analytics/analytics-report-export-success.png" alt="Confirmación de reporte analítico exportado" width="175"> |

#### 3.1.4.1.6. Governance

Governance agrupa la supervisión de cumplimiento y la atención de alertas. El dashboard resume el estado institucional y los protocolos activos; la vista de alertas prioriza bloqueos y riesgos, explica su causa y propone una acción. La combinación de prioridad textual, descripción e intervención reduce la dependencia de señales cromáticas y facilita decidir qué atender primero.

| Supervisión de gobernanza | Resolución de alertas |
|:--:|:--:|
| <img src="assets/images/chapter-3/application-ux-ui-design/application-wireframes/governance/governance-dashboard.png" alt="Dashboard de gobernanza, cumplimiento y protocolos" width="175"> | <img src="assets/images/chapter-3/application-ux-ui-design/application-wireframes/governance/active-alerts-resolution.png" alt="Cola priorizada de alertas con causas y acciones recomendadas" width="175"> |

#### 3.1.4.1.7. Profile

Profile reúne la información de la cuenta, las preferencias y los controles de seguridad. Desde el perfil se accede a la edición de la cuenta, a la actualización de la fotografía y a la confirmación de cierre de sesión. Los estados de éxito hacen explícito cuándo los cambios quedaron guardados; separar estas acciones del contenido de Projects y Governance mantiene una arquitectura predecible.

| Perfil | Editar cuenta y seguridad | Actualizar fotografía |
|:--:|:--:|:--:|
| <img src="assets/images/chapter-3/application-ux-ui-design/application-wireframes/profile/profile-overview.png" alt="Vista general del perfil y sus preferencias" width="175"> | <img src="assets/images/chapter-3/application-ux-ui-design/application-wireframes/profile/account-security-edit-modal.png" alt="Edición de cuenta, acceso y seguridad" width="175"> | <img src="assets/images/chapter-3/application-ux-ui-design/application-wireframes/profile/profile-photo-edit-modal.png" alt="Modal para actualizar la fotografía de perfil" width="175"> |

| Cambios guardados | Confirmar cierre de sesión | Cierre de sesión exitoso|
|:--:|:--:|:--:|
| <img src="assets/images/chapter-3/application-ux-ui-design/application-wireframes/profile/profile-changes-success.png" alt="Confirmación de cambios de perfil guardados" width="175"> | <img src="assets/images/chapter-3/application-ux-ui-design/application-wireframes/profile/logout-confirmation-modal.png" alt="Confirmación antes de cerrar sesión" width="175"> |<p align="center"><img src="assets/images/chapter-3/application-ux-ui-design/application-wireframes/authentication/logout-success.png" alt="Confirmación de cierre de sesión" width="175"></p>|

### 3.1.4.2. Mobile Applications Wireflow Diagrams

Los diagramas de flujo de interfaz (wireflows) muestran cómo se conectan las pantallas y acciones de Vantage PMO para que cada usuario alcance un objetivo concreto (User Goal). Cada recorrido presenta la secuencia de interacción, desde el punto de entrada hasta la respuesta del sistema, e incluye los pasos necesarios para completar la tarea. Los nueve objetivos se relacionan con las User Stories (US) del capítulo II cuando corresponde; también se incluyen flujos complementarios de autenticación, registro y gestión de cuenta para representar de forma integral la experiencia móvil.

<table width="100%">
	<tr>
		<th width="30%">User Goal</th>
		<th width="70%">Wireflow</th>
	</tr>
	<tr>
		<td><strong>UG-01 — Gestión de acceso a la cuenta.</strong> Como usuario, quiero iniciar sesión o recuperar mi contraseña, para acceder de forma segura a Vantage PMO. El recorrido comienza en la pantalla de acceso; si el usuario no recuerda su contraseña, solicita un código por correo, lo valida y define una nueva. El flujo concluye con la confirmación de actualización, dejando la cuenta disponible para iniciar sesión.</td>
		<td>
			<img src="assets/images/chapter-3/application-ux-ui-design/application-wireflow-diagrams/ug-01-authentication.png" alt="Wireflow de acceso y recuperación de cuenta" width="100%">
		</td>
	</tr>
	<tr>
		<td><strong>UG-02 — Registro de usuario.</strong> Como visitante, quiero crear una cuenta y completar mis datos, para comenzar a utilizar Vantage PMO con un perfil adecuado a mis responsabilidades. El proceso organiza la información personal, los datos de contacto y acceso, y el perfil profesional en pasos consecutivos; luego permite seleccionar un rol. La confirmación final comunica que el registro se completó.</td>
		<td>
			<img src="assets/images/chapter-3/application-ux-ui-design/application-wireflow-diagrams/ug-02-user-registration.png" alt="Wireflow de registro de cuenta" width="100%">
		</td>
	</tr>
	<tr>
		<td><strong>UG-03 — Consulta móvil del portafolio.</strong> Como Project Manager, quiero consultar el estado del portafolio desde el móvil, para detectar avances y desviaciones. El recorrido parte del dashboard, donde se resumen indicadores y alertas; continúa en la lista de proyectos y permite profundizar en el roadmap. Así, el usuario pasa de una vista general a la planificación de iniciativas bajo su responsabilidad. (US03, US14)</td>
		<td>
			<img src="assets/images/chapter-3/application-ux-ui-design/application-wireflow-diagrams/ug-03-mobile-portfolio-overview.png" alt="Wireflow de consulta del portafolio móvil" width="100%">
		</td>
	</tr>
	<tr>
		<td><strong>UG-04 — Registro de proyecto.</strong> Como Project Manager, quiero registrar un proyecto con su información principal, para iniciar su planificación y seguimiento. El usuario parte de la lista de proyectos, completa el formulario de creación y revisa la confirmación con los datos de la nueva iniciativa. El proyecto queda incorporado al espacio de trabajo para continuar con su gestión. (US01)</td>
		<td>
			<img src="assets/images/chapter-3/application-ux-ui-design/application-wireflow-diagrams/ug-04-project-registration.png" alt="Wireflow de registro de proyecto" width="100%">
		</td>
	</tr>
	<tr>
		<td><strong>UG-05 — Gestión de tareas en Kanban.</strong> Como Project Manager, quiero crear y asignar tareas, para organizar el trabajo del equipo. Desde el tablero del proyecto, el usuario abre el formulario contextual, registra la tarea y define la información necesaria para asignarla. El flujo concluye con su incorporación al tablero y una confirmación visible. (US04)</td>
		<td>
			<img src="assets/images/chapter-3/application-ux-ui-design/application-wireflow-diagrams/ug-05-task-assignment-kanban.png" alt="Wireflow de creación y asignación de tareas en Kanban" width="100%">
		</td>
	</tr>
	<tr>
		<td><strong>UG-06 — Análisis y generación de reportes.</strong> Como Project Manager, quiero consultar indicadores y generar reportes, para evaluar el desempeño de los proyectos. El usuario revisa los KPIs y sus filtros, selecciona las opciones de exportación y solicita el reporte. Una confirmación informa que la descarga se completó y que el resultado está disponible para su consulta. (US11, US12)</td>
		<td>
			<img src="assets/images/chapter-3/application-ux-ui-design/application-wireflow-diagrams/ug-06-kpi-reporting.png" alt="Wireflow de consulta de indicadores y generación de reportes" width="100%">
		</td>
	</tr>
	<tr>
		<td><strong>UG-07 — Seguimiento de alertas y riesgos.</strong> Como Project Manager, quiero revisar alertas y riesgos, para actuar oportunamente ante eventos que puedan afectar los proyectos. Desde el dashboard de Governance, el usuario accede a las alertas activas, revisa su prioridad y contexto, y consulta las acciones propuestas. El flujo facilita decidir qué situación requiere atención primero. (US07, US13)</td>
		<td>
			<img src="assets/images/chapter-3/application-ux-ui-design/application-wireflow-diagrams/ug-07-governance-alerts-risks.png" alt="Wireflow de revisión de alertas y riesgos" width="100%">
		</td>
	</tr>
	<tr>
		<td><strong>UG-08 — Actualización del perfil.</strong> Como usuario registrado, quiero actualizar mis datos personales o mi fotografía, para mantener vigente la información de mi cuenta. Desde la vista de perfil, el usuario accede a la edición correspondiente, realiza los cambios y los guarda. La confirmación final indica que la actualización se completó correctamente.</td>
		<td>
			<img src="assets/images/chapter-3/application-ux-ui-design/application-wireflow-diagrams/ug-08-profile-update.png" alt="Wireflow de actualización del perfil" width="100%">
		</td>
	</tr>
	<tr>
		<td><strong>UG-09 — Cierre de sesión.</strong> Como usuario autenticado, quiero cerrar mi sesión de forma segura, para proteger el acceso a mi cuenta cuando termine de utilizar la aplicación. El usuario inicia la acción desde su perfil y confirma su decisión en el diálogo correspondiente. El flujo termina en la pantalla de cierre exitoso y deja la sesión finalizada.</td>
		<td>
			<img src="assets/images/chapter-3/application-ux-ui-design/application-wireflow-diagrams/ug-09-logout.png" alt="Wireflow de cierre de sesión" width="100%">
		</td>
	</tr>
</table>

### 3.1.4.3. Mobile Applications Mock-ups

Los siguientes mockups presentan la propuesta visual de Vantage PMO en un dispositivo móvil. A diferencia de los wireframes, muestran la aplicación de color, tipografía, iconografía, componentes y estados de interacción con mayor nivel de detalle. Se organizan según las áreas de uso para facilitar la lectura de las pantallas principales y sus variantes.

#### 3.1.4.3.1. Authentication

Este flujo reúne el inicio de la aplicación, el acceso y la recuperación de contraseña. También incluye el cierre de sesión exitoso como estado de salida de la cuenta.

| Inicio | Inicio de sesión | Recuperación por correo |
|:--:|:--:|:--:|
| <img src="assets/images/chapter-3/application-ux-ui-design/application-mockups/authentication/mobile-splash-screen.png" alt="Mockup de inicio de Vantage PMO" width="150"> | <img src="assets/images/chapter-3/application-ux-ui-design/application-mockups/authentication/login-screen.png" alt="Mockup de inicio de sesión" width="150"> | <img src="assets/images/chapter-3/application-ux-ui-design/application-mockups/authentication/password-recovery-email.png" alt="Mockup de recuperación de contraseña por correo" width="150"> |

| Verificación del código | Nueva contraseña | Recuperación completada |
|:--:|:--:|:--:|
| <img src="assets/images/chapter-3/application-ux-ui-design/application-mockups/authentication/password-recovery-verification-code.png" alt="Mockup de verificación del código" width="150"> | <img src="assets/images/chapter-3/application-ux-ui-design/application-mockups/authentication/password-recovery-new-password.png" alt="Mockup de creación de nueva contraseña" width="150"> | <img src="assets/images/chapter-3/application-ux-ui-design/application-mockups/authentication/password-recovery-success.png" alt="Mockup de confirmación de contraseña actualizada" width="150"> |

#### 3.1.4.3.2. Registration

El registro se presenta como un proceso progresivo, con indicadores de avance y formularios separados por tipo de información. La última pantalla confirma la creación de la cuenta y resume el perfil configurado.

| Datos personales | Contacto y acceso | Perfil profesional |
|:--:|:--:|:--:|
| <img src="assets/images/chapter-3/application-ux-ui-design/application-mockups/registration/personal-information.png" alt="Mockup del paso de datos personales" width="150"> | <img src="assets/images/chapter-3/application-ux-ui-design/application-mockups/registration/contact-and-access.png" alt="Mockup del paso de contacto y acceso" width="150"> | <img src="assets/images/chapter-3/application-ux-ui-design/application-mockups/registration/professional-profile.png" alt="Mockup del paso de perfil profesional" width="150"> |

| Selección de rol | Registro completado |
|:--:|:--:|
| <img src="assets/images/chapter-3/application-ux-ui-design/application-mockups/registration/role-selection.png" alt="Mockup de selección de rol" width="150"> | <img src="assets/images/chapter-3/application-ux-ui-design/application-mockups/registration/registration-success.png" alt="Mockup de cuenta creada" width="150"> |

#### 3.1.4.3.3. Dashboard

La pantalla principal combina una alerta prioritaria con indicadores del portafolio, hitos, salud de proyectos y capacidad del equipo. La navegación inferior mantiene el acceso a las áreas centrales de la aplicación.

<p align="center"><img src="assets/images/chapter-3/application-ux-ui-design/application-mockups/dashboard/home-dashboard.png" alt="Mockup del dashboard móvil con alerta prioritaria e indicadores" width="190"></p>

#### 3.1.4.3.4. Projects

Projects concentra la consulta del portafolio, el registro de iniciativas y la gestión del trabajo en Kanban. También presenta las opciones de exportación y la planificación estratégica mediante el roadmap.

| Lista de proyectos | Crear proyecto | Proyecto creado |
|:--:|:--:|:--:|
| <img src="assets/images/chapter-3/application-ux-ui-design/application-mockups/projects/project-list.png" alt="Mockup de la lista de proyectos" width="150"> | <img src="assets/images/chapter-3/application-ux-ui-design/application-mockups/projects/project-creation-form.png" alt="Mockup del formulario de creación de proyecto" width="150"> | <img src="assets/images/chapter-3/application-ux-ui-design/application-mockups/projects/project-creation-success.png" alt="Mockup de confirmación de proyecto creado" width="150"> |

| Tablero Kanban | Crear tarea | Tarea registrada |
|:--:|:--:|:--:|
| <img src="assets/images/chapter-3/application-ux-ui-design/application-mockups/projects/kanban-board.png" alt="Mockup del tablero Kanban" width="150"> | <img src="assets/images/chapter-3/application-ux-ui-design/application-mockups/projects/kanban-task-creation-modal.png" alt="Mockup del formulario de creación de tarea" width="150"> | <img src="assets/images/chapter-3/application-ux-ui-design/application-mockups/projects/task-creation-success.png" alt="Mockup de confirmación de tarea registrada" width="150"> |

| Exportar reporte | Dossier exportado | Roadmap estratégico |
|:--:|:--:|:--:|
| <img src="assets/images/chapter-3/application-ux-ui-design/application-mockups/projects/strategic-roadmap.png" alt="Mockup del roadmap estratégico" width="150">  | <img src="assets/images/chapter-3/application-ux-ui-design/application-mockups/projects/project-dossier-export-success.png" alt="Mockup de confirmación de dossier exportado" width="150"> | <img src="assets/images/chapter-3/application-ux-ui-design/application-mockups/projects/project-report-export-modal.png" alt="Mockup del modal de exportación de reporte" width="150"> |

#### 3.1.4.3.5. Analytics

Analytics ofrece una vista de indicadores de desempeño, filtros temporales y opciones de exportación. El estado de éxito muestra la confirmación de generación y descarga del dossier ejecutivo.

| Indicadores | Configurar exportación | Exportación completada |
|:--:|:--:|:--:|
| <img src="assets/images/chapter-3/application-ux-ui-design/application-mockups/analytics/analytics-dashboard.png" alt="Mockup de analítica con indicadores de desempeño" width="150"> | <img src="assets/images/chapter-3/application-ux-ui-design/application-mockups/analytics/analytics-report-export-modal.png" alt="Mockup de opciones de exportación analítica" width="150"> | <img src="assets/images/chapter-3/application-ux-ui-design/application-mockups/analytics/analytics-report-export-success.png" alt="Mockup de reporte analítico exportado" width="150"> |

#### 3.1.4.3.6. Governance

Governance reúne el estado de cumplimiento institucional y la atención de bloqueos. La segunda pantalla prioriza alertas, expone sus causas y ofrece acciones de mitigación.

| Supervisión de gobernanza | Resolución de alertas |
|:--:|:--:|
| <img src="assets/images/chapter-3/application-ux-ui-design/application-mockups/governance/governance-dashboard.png" alt="Mockup del dashboard de gobernanza y cumplimiento" width="150"> | <img src="assets/images/chapter-3/application-ux-ui-design/application-mockups/governance/active-alerts-resolution.png" alt="Mockup de alertas activas y acciones de resolución" width="150"> |

#### 3.1.4.3.7. Profile

Profile centraliza la información de la cuenta, las opciones de seguridad y las preferencias. Los mockups incluyen la edición de datos, el cambio de fotografía, la confirmación de modificaciones y el diálogo previo al cierre de sesión.

| Perfil | Editar cuenta y seguridad | Actualizar fotografía |
|:--:|:--:|:--:|
| <img src="assets/images/chapter-3/application-ux-ui-design/application-mockups/profile/profile-overview.png" alt="Mockup de vista general del perfil" width="150"> | <img src="assets/images/chapter-3/application-ux-ui-design/application-mockups/profile/account-security-edit-modal.png" alt="Mockup de edición de cuenta y seguridad" width="150"> | <img src="assets/images/chapter-3/application-ux-ui-design/application-mockups/profile/profile-photo-edit-modal.png" alt="Mockup de actualización de fotografía de perfil" width="150"> |

| Cambios guardados | Confirmar cierre de sesión | Cierre de sesión exitoso |
|:--:|:--:|:--:|
| <img src="assets/images/chapter-3/application-ux-ui-design/application-mockups/profile/profile-changes-success.png" alt="Mockup de confirmación de cambios guardados" width="150"> | <img src="assets/images/chapter-3/application-ux-ui-design/application-mockups/profile/logout-confirmation-modal.png" alt="Mockup de confirmación de cierre de sesión" width="150"> |<p align="center"><img src="assets/images/chapter-3/application-ux-ui-design/application-mockups/authentication/logout-success.png" alt="Mockup de cierre de sesión exitoso" width="150"></p>|

### 3.1.4.4. Mobile Applications User Flow Diagrams

Esta sección presenta la propuesta de User Flows para la aplicación móvil Vantage PMO. Se define un flujo para cada User Goal, considerando las personas usuarias involucradas —visitante, usuario registrado y Project Manager— y manteniendo la correspondencia con los Wireflows de la sección anterior. Los diagramas incorporan los mock-ups de las pantallas, la ruta esperada (happy path) y las rutas alternativas o condiciones que pueden interrumpir o desviar el recorrido (unhappy paths). Se elaboraron con la herramienta de diseño indicada para la propuesta (Figma). Cada flujo incluye el objetivo del usuario y una explicación de sus pasos y decisiones.

<table width="100%">
	<tr>
		<th width="35%">User Goal y explicación</th>
		<th width="65%">User Flow</th>
	</tr>
	<tr>
		<td><strong>UG-01 — Gestión de acceso a la cuenta.</strong> Como usuario, quiero iniciar sesión o recuperar mi contraseña, para acceder de forma segura a Vantage PMO.<br><br><strong>Happy path:</strong> desde el acceso, el usuario solicita recuperar la contraseña, recibe y verifica el código enviado a su correo, define una contraseña nueva y llega a la confirmación. <strong>Alternativas:</strong> si no recibe el código, puede solicitar su reenvío; si el código o los datos no son válidos, debe corregirlos o volver a solicitarlo antes de continuar. También puede volver al acceso e iniciar sesión.</td>
		<td><img src="assets/images/chapter-3/application-ux-ui-design/application-user-flow-diagrams/ug-01-authentication.png" alt="User Flow de acceso y recuperación de cuenta" width="100%"></td>
	</tr>
	<tr>
		<td><strong>UG-02 — Registro de usuario.</strong> Como visitante, quiero crear una cuenta y completar mis datos, para comenzar a utilizar Vantage PMO con un perfil adecuado a mis responsabilidades.<br><br><strong>Happy path:</strong> completa los datos personales, de contacto y acceso, y el perfil profesional; selecciona un rol y recibe la confirmación de la cuenta creada. <strong>Alternativas:</strong> los datos obligatorios incompletos o no válidos deben corregirse en el paso correspondiente antes de avanzar; el usuario puede permanecer en el formulario y completar la información pendiente.</td>
		<td><img src="assets/images/chapter-3/application-ux-ui-design/application-user-flow-diagrams/ug-02-user-registration.png" alt="User Flow de registro de usuario" width="100%"></td>
	</tr>
	<tr>
		<td><strong>UG-03 — Consulta móvil del portafolio.</strong> Como Project Manager, quiero consultar el estado del portafolio desde el móvil, para detectar avances y desviaciones.<br><br><strong>Happy path:</strong> revisa los indicadores y alertas del dashboard, abre la lista de proyectos y profundiza en el roadmap para consultar la planificación. <strong>Alternativas:</strong> puede permanecer en la vista general o ajustar los filtros y periodos disponibles para enfocar la consulta antes de abrir un proyecto o el roadmap.</td>
		<td><img src="assets/images/chapter-3/application-ux-ui-design/application-user-flow-diagrams/ug-03-mobile-portfolio-overview.png" alt="User Flow de consulta móvil del portafolio" width="100%"></td>
	</tr>
	<tr>
		<td><strong>UG-04 — Registro de proyecto.</strong> Como Project Manager, quiero registrar un proyecto con su información principal, para iniciar su planificación y seguimiento.<br><br><strong>Happy path:</strong> parte de la lista de proyectos, completa la información de la iniciativa y sus datos de planificación, y consulta la confirmación de creación. <strong>Alternativas:</strong> si faltan datos requeridos o no son válidos, debe corregir el formulario antes de registrar el proyecto; también puede salir del formulario sin completar el alta.</td>
		<td><img src="assets/images/chapter-3/application-ux-ui-design/application-user-flow-diagrams/ug-04-project-registration.png" alt="User Flow de registro de proyecto" width="100%"></td>
	</tr>
	<tr>
		<td><strong>UG-05 — Gestión de tareas en Kanban.</strong> Como Project Manager, quiero crear y asignar tareas, para organizar el trabajo del equipo.<br><br><strong>Happy path:</strong> abre el tablero del proyecto, crea una tarea, define su información y responsables, y recibe confirmación de que quedó registrada. <strong>Alternativas:</strong> si falta información necesaria para registrar o asignar la tarea, debe completarla antes de confirmar; puede cancelar la creación y regresar al tablero sin guardar.</td>
		<td><img src="assets/images/chapter-3/application-ux-ui-design/application-user-flow-diagrams/ug-05-task-assignment-kanban.png" alt="User Flow de creación y asignación de tareas en Kanban" width="100%"></td>
	</tr>
	<tr>
		<td><strong>UG-06 — Análisis y generación de reportes.</strong> Como Project Manager, quiero consultar indicadores y generar reportes, para evaluar el desempeño de los proyectos.<br><br><strong>Happy path:</strong> revisa los KPIs, selecciona el periodo y formato de exportación, solicita el reporte y recibe la confirmación de descarga. <strong>Alternativas:</strong> puede cambiar el periodo o formato, o cancelar la exportación y volver a los indicadores; si la generación no se completa, el flujo no muestra un éxito y permite volver a intentarlo.</td>
		<td><img src="assets/images/chapter-3/application-ux-ui-design/application-user-flow-diagrams/ug-06-kpi-reporting.png" alt="User Flow de análisis y generación de reportes" width="100%"></td>
	</tr>
	<tr>
		<td><strong>UG-07 — Seguimiento de alertas y riesgos.</strong> Como Project Manager, quiero revisar alertas y riesgos, para actuar oportunamente ante eventos que puedan afectar los proyectos.<br><br><strong>Happy path:</strong> accede desde Governance a la cola de alertas, revisa la prioridad, la causa y la acción recomendada, y aplica la mitigación o marca la alerta como atendida. <strong>Alternativas:</strong> si la acción requiere autorización, puede dejarla pendiente o reasignarla a una persona responsable; también puede revisar otra alerta antes de actuar.</td>
		<td><img src="assets/images/chapter-3/application-ux-ui-design/application-user-flow-diagrams/ug-07-governance-alerts-risks.png" alt="User Flow de revisión de alertas y riesgos" width="100%"></td>
	</tr>
	<tr>
		<td><strong>UG-08 — Actualización del perfil.</strong> Como usuario registrado, quiero actualizar mis datos personales o mi fotografía, para mantener vigente la información de mi cuenta.<br><br><strong>Happy path:</strong> desde el perfil, elige editar los datos de la cuenta o actualizar la fotografía, guarda los cambios y recibe una confirmación. <strong>Alternativas:</strong> puede cancelar la edición para conservar la información actual; si los datos no superan la validación, debe corregirlos antes de guardar.</td>
		<td><img src="assets/images/chapter-3/application-ux-ui-design/application-user-flow-diagrams/ug-08-profile-update.png" alt="User Flow de actualización del perfil" width="100%"></td>
	</tr>
	<tr>
		<td><strong>UG-09 — Cierre de sesión.</strong> Como usuario autenticado, quiero cerrar mi sesión de forma segura, para proteger el acceso a mi cuenta cuando termine de utilizar la aplicación.<br><br><strong>Happy path:</strong> inicia el cierre desde el perfil y confirma la acción en el diálogo; el recorrido termina en la pantalla de cierre exitoso. <strong>Alternativa:</strong> si cancela o descarta el diálogo, vuelve al perfil y conserva su sesión activa.</td>
		<td><img src="assets/images/chapter-3/application-ux-ui-design/application-user-flow-diagrams/ug-09-logout.png" alt="User Flow de cierre de sesión" width="100%"></td>
	</tr>
</table>

### 3.1.4.5. Mobile Applications Prototyping
*(Insertar enlaces al video de Figma)*