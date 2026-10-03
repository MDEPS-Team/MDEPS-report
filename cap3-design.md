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

**Arquitectura de información.** Antes de iniciar sesión, la información se organiza en acceso, recuperación de credenciales y creación de cuenta. Después de autenticarse, una navegación persistente agrupa las áreas principales en Home, Projects, Analytics, Governance y Profile. Dentro de cada área, la jerarquía conduce de la vista general a una tarea concreta —por ejemplo, seleccionar un proyecto, revisar una alerta o editar la cuenta— y presenta confirmaciones al completar acciones relevantes. Esta organización responde a la necesidad identificada de consultar desde el móvil el estado de los proyectos, sus responsables, fechas, indicadores y alertas desde un punto centralizado.

#### 3.1.4.1.1. Authentication

El recorrido de autenticación comienza con la pantalla de inicio de Vantage PMO y el formulario de acceso. Si el usuario no recuerda sus credenciales, puede solicitar un código, verificarlo, definir una nueva contraseña y confirmar la actualización. La secuencia hace visible el paso actual y ofrece una confirmación final; la pantalla de cierre exitoso comunica que la sesión terminó.

| Inicio de la aplicación | Acceso | Recuperación por correo |
|:--:|:--:|:--:|
| <img src="assets/images/chapter-3/application-ux-ui-design/application-wireframes/authentication/mobile-splash-screen.png" alt="Pantalla de inicio de Vantage PMO" width="175"> | <img src="assets/images/chapter-3/application-ux-ui-design/application-wireframes/authentication/login-screen.png" alt="Formulario de inicio de sesión" width="175"> | <img src="assets/images/chapter-3/application-ux-ui-design/application-wireframes/authentication/password-recovery-email.png" alt="Solicitud de recuperación de contraseña por correo" width="175"> |

| Verificación del código | Nueva contraseña | Recuperación completada |
|:--:|:--:|:--:|
| <img src="assets/images/chapter-3/application-ux-ui-design/application-wireframes/authentication/password-recovery-verification-code.png" alt="Verificación del código de seguridad" width="175"> | <img src="assets/images/chapter-3/application-ux-ui-design/application-wireframes/authentication/password-recovery-new-password.png" alt="Formulario para crear una contraseña nueva" width="175"> | <img src="assets/images/chapter-3/application-ux-ui-design/application-wireframes/authentication/password-recovery-success.png" alt="Confirmación de contraseña actualizada" width="175"> |


#### 3.1.4.1.2. Registration

El registro se divide en cuatro pasos —datos personales, contacto y acceso, perfil profesional y selección de rol— seguidos por una pantalla de cuenta creada. El indicador numerado permite reconocer el avance y anticipar cuánto falta; la agrupación de campos reduce la carga de cada pantalla. La selección de rol introduce una arquitectura personalizada según las responsabilidades del usuario dentro de la PMO.

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
### 3.1.4.3. Mobile Applications Mock-ups
### 3.1.4.4. Mobile Applications User Flow Diagrams
### 3.1.4.5. Mobile Applications Prototyping
*(Insertar enlaces al video de Figma)*