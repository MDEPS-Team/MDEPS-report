# Capitulo II: Requirements Development and Software Solution Design

## 2.1. Competidores

### 2.1.1. Analisis competitivo
| ¿Por que llevar a cabo este analisis? | [Explicar el proposito del analisis competitivo] | | | |
| :--- | :--- | :--- | :--- | :--- |
| **Startups** | **FlowAlert (Propuesta)** | **Competidor 1** | **Competidor 2** | **Competidor 3** |
| **Overview** | [Descripcion] | [Descripcion] | [Descripcion] | [Descripcion] |
| **Ventaja Competitiva** | [Diferenciador] | [Diferenciador] | [Diferenciador] | [Diferenciador] |
| **Mercado Objetivo** | [Target] | [Target] | [Target] | [Target] |
| **Estrategias de Marketing**| [Estrategia] | [Estrategia] | [Estrategia] | [Estrategia] |
| **Productos & Servicios** | [Servicios] | [Servicios] | [Servicios] | [Servicios] |
| **Precios & Costos** | [Modelo de precio] | [Modelo de precio] | [Modelo de precio] | [Modelo de precio] |
| **Canales de Distribucion** | [Canales] | [Canales] | [Canales] | [Canales] |
| **Fortalezas (SWOT)** | [Fortalezas] | [Fortalezas] | [Fortalezas] | [Fortalezas] |
| **Debilidades (SWOT)** | [Debilidades] | [Debilidades] | [Debilidades] | [Debilidades] |
| **Oportunidades (SWOT)**| [Oportunidades] | [Oportunidades] | [Oportunidades] | [Oportunidades] |
| **Amenazas (SWOT)** | [Amenazas] | [Amenazas] | [Amenazas] | [Amenazas] |

### 2.1.2. Estrategias y tacticas frente a competidores
[Detallar estrategias y tacticas para aprovechar brechas de la competencia].

---

## 2.2. Entrevistas

### 2.2.1. Diseno de entrevistas
[Colocar preguntas por cada segmento objetivo].

### 2.2.2. Registro de entrevistas
- **Entrevista 1:**
  - Nombres y Apellidos: [Datos]
  - Edad / Ubicacion: [Datos]
  - URL del Video: [Enlace OneDrive]
  - Screenshot: [Imagen de video con timing visible]
  - Resumen: [Resumen descriptivo con variables objetivas y subjetivas]

### 2.2.3. Analisis de entrevistas
[Tablas con sustento porcentual y caracteristicas mas comunes detectadas].

---

## 2.3. Needfinding

### 2.3.1. User Personas
[Insertar fichas exportadas de UXPressia para cada segmento].

### 2.3.2. User Task Matrix
| Tarea | Frecuencia (Persona 1) | Importancia (Persona 1) | Frecuencia (Persona 2) | Importancia (Persona 2) |
| :--- | :--- | :--- | :--- | :--- |
| [Tarea 1] | Alta / Media / Baja | Alta / Media / Baja | Alta / Media / Baja | Alta / Media / Baja |

### 2.3.3. User Journey Mapping
[Insertar diagramas As-Is elaborados en UXPressia].

### 2.3.4. Empathy Mapping
[Insertar mapas de empatia por segmento].

### 2.3.5. Big Picture EventStorming
[Capturas de la sesion en Miro y explicacion del flujo temporal general de eventos de dominio].

### 2.3.6. Ubiquitous Language
[Glosario de terminos en ingles con definicion en espanol]:
- **Termino en ingles (Traduccion):** Definicion conceptual del dominio de negocio.

---

## 2.4. Requirements Specification

### 2.4.1. User Stories
[Listar Epics, User Stories con formato Gherkin, Spike Stories y Technical Stories]:

| Story ID: US01 | User: [Rol] | Priority: [Alta/Media/Baja] | Epic: EP01 |
| :--- | :--- | :--- | :--- |
| **Title** | [Titulo de la User Story] |
| **Description** | Como [rol], quiero [accion] para [beneficio]. |
| **Acceptance Criteria** | **Escenario 1:**<br>Dado que [contexto],<br>Cuando [evento],<br>Entonces [resultado esperado]. |

### 2.4.2. Impact Mapping
[Captura del Impact Map elaborado en herramienta visual].

### 2.4.3. Product Backlog
| # Orden | User Story ID | Titulo | Story Points | Sprint |
| :--- | :--- | :--- | :--- | :--- |
| 1 | [ID] | [Titulo] | [Puntaje] | [Sprint] |

---

## 2.5. Strategic-Level Domain-Driven Design

### 2.5.1. EventStorming
[Explicacion del proceso colaborativo].

#### 2.5.1.1. Candidate Context Discovery
[Identificacion de Bounded Contexts candidatos].

#### 2.5.1.2. Domain Message Flows Modeling
[Diagramas de Domain Storytelling / flujo de mensajes].

#### 2.5.1.3. Bounded Context Canvases
[Lienzos Bounded Context Canvas por cada contexto].

### 2.5.2. Context Mapping
[Diagrama con relaciones Upstream, Downstream, ACL, Conformist, Customer-Supplier].

### 2.5.3. Software Architecture
#### 2.5.3.1. Software Architecture Context Level Diagrams
[Diagrama C4 Nivel 1 Context Diagram y descripcion].

#### 2.5.3.2. Software Architecture Container Level Diagrams
[Diagrama C4 Nivel 2 Container Diagram y descripcion].

#### 2.5.3.3. Software Architecture Deployment Diagrams
[Diagrama C4 de Despliegue de infraestructura y descripcion].

---

## 2.6. Tactical-Level Domain-Driven Design

### 2.6.1. Bounded Context: IAM

Siguiendo el modelo de arquitectura "Clean Architecture", hemos dividido el proyecto en capas. A continuación detallamos las capas del Bounded Context referenciado.

#### 2.6.1.1. Domain Layer

**Sub-capa Model - Aggregates:**

| Tipo | Nombre | Descripción | Responsabilidad Principal | Relación con otros elementos |
| :--- | :--- | :--- | :--- | :--- |
| Aggregate | User | Clase para definir el Usuario de la aplicación. | Ser el punto de entrada para modificar y mantener la integridad del usuario como entidad del dominio de identidad. | Relacionado con los demás bounded contexts, ya que encapsula la identidad principal del sistema. |
| Aggregate | UserAudit | Clase para definir la auditoría de los usuarios. | Mantener el registro y la traza de los eventos críticos relacionados con los usuarios. | Relacionado directamente con la entidad `User`. |

**Sub-capa Model - Commands:**

| Tipo | Nombre | Descripción | Responsabilidad Principal | Relación con otros elementos |
| :--- | :--- | :--- | :--- | :--- |
| Command | SignInCommand | Comando para el inicio de sesión. | Representar la intención del usuario de iniciar sesión en el sistema. | Usado en la implementación del servicio de autenticación (Application Layer). |
| Command | SignUpCommand | Comando para registro. | Representar la intención de un nuevo usuario de registrarse en la aplicación. | Usado en la implementación del servicio de autenticación (Application Layer). |
| Command | UpdatePasswordCommand | Comando para actualizar credenciales. | Representar la intención de un usuario de cambiar su contraseña de acceso. | Usado en la implementación de la gestión de usuarios. |

**Sub-capa Model - Queries:**

| Tipo | Nombre | Descripción | Responsabilidad Principal | Relación con otros elementos |
| :--- | :--- | :--- | :--- | :--- |
| Query | GetAllUsersQuery | Consulta para obtener todos los usuarios. | Representar la intención de obtener la lista completa de usuarios registrados. | Usado en la implementación del servicio de consultas (UserQueryService). |
| Query | GetUserByIdQuery | Consulta para obtener un usuario por ID. | Representar la intención de buscar los detalles de un usuario específico mediante su identificador. | Usado en la implementación del servicio de consultas. |
| Query | GetUserByUsernameQuery | Consulta para obtener un usuario por su Username. | Representar la intención de buscar un usuario utilizando su nombre de usuario. | Usado en la validación y el servicio de consultas de autenticación. |

**Sub-capa Repositories:**

| Tipo | Nombre | Descripción | Responsabilidad Principal | Relación con otros elementos |
| :--- | :--- | :--- | :--- | :--- |
| Repository | IUserRepository | Interfaz de persistencia para la entidad User. | Definir el contrato para guardar, actualizar y recuperar información de la base de datos para los usuarios. | Implementado por `UserRepository` en la capa de Infraestructura (Infrastructure Layer). |

#### 2.6.1.2. Interface Layer

**Sub-capa REST - Resources:**

| Tipo | Nombre | Descripción | Responsabilidad Principal | Relación con otros elementos |
| :--- | :--- | :--- | :--- | :--- |
| Resource | UserResource | Representación del recurso de usuario. | Definir la estructura de datos que se expone al cliente cuando se consulta un usuario. | Relacionado con `UserResourceFromEntityAssembler` para transformar entidades del dominio a recursos. |
| Resource | AuthenticatedUserResource | Representación de un usuario autenticado. | Definir la estructura de datos expuesta al cliente luego de un inicio de sesión exitoso (incluye token). | Utilizado en las respuestas de autenticación y relacionado con `AuthenticatedUserResourceFromEntityAssembler`. |
| Resource | SignInResource | Representación de los datos para iniciar sesión. | Capturar los datos enviados por el cliente (ej. username y contraseña) para la autenticación. | Transformado a `SignInCommand` a través de `SignInCommandFromResourceAssembler`. |
| Resource | SignUpResource | Representación de los datos para el registro. | Capturar los datos enviados por el cliente para crear una nueva cuenta. | Transformado a `SignUpCommand` a través de `SignUpCommandFromResourceAssembler`. |
| Resource | FrontSignInUserResource | Representación adaptada para el frontend del inicio de sesión. | Estructura específica para las necesidades del frontend al iniciar sesión. | Utilizado por los controladores de autenticación. |
| Resource | FrontSignUpResource | Representación adaptada para el frontend del registro. | Estructura específica para las necesidades del frontend al crear cuenta. | Utilizado por los controladores de autenticación. |
| Resource | FrontPatchUserResource | Representación adaptada para actualizaciones desde el frontend. | Capturar datos enviados para actualización parcial de usuario. | Utilizado por los controladores para operaciones de parcheo. |

**Sub-capa REST - Transform:**

| Tipo | Nombre | Descripción | Responsabilidad Principal | Relación con otros elementos |
| :--- | :--- | :--- | :--- | :--- |
| Assembler | SignInCommandFromResourceAssembler | Ensamblador de comandos de inicio de sesión. | Transformar un `SignInResource` proveniente de la petición HTTP en un `SignInCommand` para la capa de aplicación. | Relaciona recursos HTTP con comandos de dominio. |
| Assembler | SignUpCommandFromResourceAssembler | Ensamblador de comandos de registro. | Transformar un `SignUpResource` en un `SignUpCommand` para ser procesado. | Relaciona recursos HTTP con comandos de dominio. |
| Assembler | FrontSignUpCommandFromResourceAssembler | Ensamblador de comandos de registro adaptado. | Transformar un `FrontSignUpResource` en comandos procesables. | Relaciona peticiones del frontend con la lógica de negocio. |
| Assembler | UserResourceFromEntityAssembler | Ensamblador de recursos de usuario. | Transformar una entidad `User` del dominio en un `UserResource` para la respuesta HTTP. | Permite exponer datos sin exponer la entidad de dominio directamente. |
| Assembler | AuthenticatedUserResourceFromEntityAssembler | Ensamblador de recursos de usuario autenticado. | Transformar la información de un usuario y su token en un `AuthenticatedUserResource`. | Prepara la respuesta de inicio de sesión exitoso. |
| Assembler | IamActionResultAssembler | Ensamblador de resultados de acciones IAM. | Estandarizar la creación de respuestas HTTP (ActionResults) para operaciones de identidad. | Usado por los controladores para retornar las respuestas adecuadas. |

**Sub-capa REST - Controllers:**

| Tipo | Nombre | Descripción | Responsabilidad Principal | Relación con otros elementos |
| :--- | :--- | :--- | :--- | :--- |
| Controller | AuthenticationController | Controlador para el manejo de autenticación. | Gestionar las peticiones HTTP relacionadas al inicio de sesión y registro de usuarios (endpoints). | Coordina con `IUserCommandService` para ejecutar comandos y usa assemblers para transformar datos. |
| Controller | UsersController | Controlador para la gestión de usuarios. | Exponer y gestionar endpoints RESTful para operaciones sobre cuentas de usuarios (listar, buscar). | Coordina con `IUserQueryService` y `IUserCommandService` para manejar flujos de datos. |

**Sub-capa ACL:**

| Tipo | Nombre | Descripción | Responsabilidad Principal | Relación con otros elementos |
| :--- | :--- | :--- | :--- | :--- |
| Facade Interface | IIamContextFacade | Interfaz de la fachada ACL para el contexto IAM. | Definir un contrato claro y aislado para que otros Bounded Contexts interactúen con IAM. | Define operaciones que pueden ser llamadas desde otros módulos (ej. Profiles, Projects). |
| Facade | IamContextFacade | Implementación de la fachada ACL para IAM. | Exponer servicios específicos de IAM (como verificar si existe un usuario) a otros Bounded Contexts, actuando como una capa anticorrupción. | Implementa `IIamContextFacade` y utiliza servicios internos de aplicación. |

#### 2.6.1.3. Application Layer

**Sub-capa Services - CommandServices:**

| Tipo | Nombre | Descripción | Responsabilidad Principal | Relación con otros elementos |
| :--- | :--- | :--- | :--- | :--- |
| Interface | IUserCommandService | Contrato para servicios de comandos de usuario. | Definir las operaciones de modificación de estado para los usuarios (ej. registro). | Implementado por `UserCommandService`. |
| Service | UserCommandService | Servicio de comandos para usuarios. | Manejar el flujo de ejecución de los comandos de escritura y modificación (`SignUpCommand`, `SignInCommand`). Contiene la lógica orquestadora. | Implementa `IUserCommandService`. Coordina con `IUserRepository`, `IHashingService` y `ITokenService`. |

**Sub-capa Services - QueryServices:**

| Tipo | Nombre | Descripción | Responsabilidad Principal | Relación con otros elementos |
| :--- | :--- | :--- | :--- | :--- |
| Interface | IUserQueryService | Contrato para servicios de consultas de usuario. | Definir las operaciones de solo lectura para obtener información de usuarios. | Implementado por `UserQueryService`. |
| Service | UserQueryService | Servicio de consultas para usuarios. | Orquestar la ejecución de consultas (queries) para recuperar datos de usuarios sin modificar su estado (ej. `GetAllUsersQuery`, `GetUserByIdQuery`). | Implementa `IUserQueryService`. Obtiene datos utilizando `IUserRepository`. |

**Sub-capa Services - OutboundServices (Internal):**

| Tipo | Nombre | Descripción | Responsabilidad Principal | Relación con otros elementos |
| :--- | :--- | :--- | :--- | :--- |
| Interface | IHashingService | Contrato para el servicio de encriptación. | Definir la funcionalidad necesaria para encriptar y verificar contraseñas. | Utilizado por `UserCommandService` para procesar credenciales seguras. Implementado en la capa de Infraestructura. |
| Interface | ITokenService | Contrato para el servicio de generación de tokens. | Definir la funcionalidad para generar tokens de autenticación (JWT) para sesiones válidas. | Utilizado por `UserCommandService` al confirmar el inicio de sesión. Implementado en la capa de Infraestructura. |

#### 2.6.1.4. Infrastructure Layer

**Sub-capa Hashing:**

| Tipo | Nombre | Descripción | Responsabilidad Principal | Relación con otros elementos |
| :--- | :--- | :--- | :--- | :--- |
| Service | HashingService | Implementación del servicio de hashing utilizando BCrypt. | Encriptar las contraseñas de los usuarios y verificar que los hashes coincidan al iniciar sesión. | Implementa `IHashingService` de la capa de Aplicación. |

**Sub-capa Persistence:**

| Tipo | Nombre | Descripción | Responsabilidad Principal | Relación con otros elementos |
| :--- | :--- | :--- | :--- | :--- |
| Repository | UserRepository | Implementación del repositorio de usuarios en Entity Framework Core. | Manejar las operaciones directas de base de datos (CRUD) para la entidad `User`. | Implementa la interfaz `IUserRepository` de la capa de Dominio. |
| Configuration | ModelBuilderExtensions | Extensiones para la configuración del modelo de datos. | Mapear las entidades del dominio de IAM (`User`, `UserAudit`) a tablas en la base de datos relacional. | Usado por el DbContext central de la aplicación. |

**Sub-capa Pipeline:**

| Tipo | Nombre | Descripción | Responsabilidad Principal | Relación con otros elementos |
| :--- | :--- | :--- | :--- | :--- |
| Middleware | RequestAuthorizationMiddleware | Interceptor de peticiones HTTP. | Interceptar cada petición entrante al servidor para extraer y validar el token JWT. | Se inyecta en el pipeline global de la aplicación. |
| Attribute | AuthorizeAttribute | Atributo de autorización. | Decorador utilizado para marcar controladores o endpoints que requieren una sesión iniciada válida. | Evaluado por el `RequestAuthorizationMiddleware`. |
| Attribute | AllowAnonymousAttribute | Atributo de omisión de autorización. | Decorador para marcar endpoints públicos que no requieren token (ej. registro). | Evaluado por el middleware para saltar la validación. |

**Sub-capa Tokens:**

| Tipo | Nombre | Descripción | Responsabilidad Principal | Relación con otros elementos |
| :--- | :--- | :--- | :--- | :--- |
| Service | TokenService | Implementación del generador de tokens JWT. | Crear tokens web de formato JSON (JWT) con claims de seguridad para la sesión. | Implementa `ITokenService` de la capa de Aplicación. |
| Configuration | TokenSettings | Configuración de los tokens. | Mapear los secretos y tiempos de expiración del JWT definidos en las configuraciones del proyecto. | Utilizado por `TokenService` para firmar los tokens. |

#### 2.6.1.5. Bounded Context Software Architecture Component Level Diagrams

Este diagrama representa la descomposición interna del contenedor correspondiente al Bounded Context de identidad y autenticación (IAM) dentro del sistema. Se ilustra en el Nivel 3 del C4 Model  para reflejar los principios de Clean Architecture y Domain-Driven Design aplicados.

En este diagrama se puede observar cómo las peticiones ingresan a través de los controladores REST (Interface Layer), los cuales delegan la lógica de negocio a los servicios de comando y consulta (Application Layer). Estos servicios, a su vez, orquestan las operaciones apoyándose en los componentes de infraestructura (Infrastructure Layer), como el repositorio para la persistencia de datos y los servicios externos para el manejo de encriptación (BCrypt) y generación de tokens (JWT).

<img width="776" height="986" alt="diagrama 1" src="https://github.com/user-attachments/assets/caa86808-2bed-40e1-8751-af3738db1fc3" />


#### 2.6.1.6. Bounded Context Software Architecture Code Level Diagrams
##### 2.6.1.6.1. Bounded Context Domain Layer Class Diagrams
<img width="1969" height="952" alt="diagrama2" src="https://github.com/user-attachments/assets/97bb35b1-aff3-4f8b-8316-c8d20974e7c2" />


##### 2.6.1.6.2. Bounded Context Database Design Diagram
<img width="203" height="385" alt="diagrama 3" src="https://github.com/user-attachments/assets/bf894c88-6d08-4a9e-9985-13a1c0a7f514" />
**Tabla: USERS**

| Campo | Tipo | Nulo | Default | Comentario / Descripción |
| :--- | :--- | :--- | :--- | :--- |
| **id** | bigint | N-N | default | Identificador único del registro, generalmente una clave primaria[cite: 2]. |
| **created_at** | datetime | NULL | default | Fecha y hora en que se creó el registro[cite: 2]. |
| **updated_at** | datetime | NULL | default | Fecha y hora de la última actualización del registro[cite: 2]. |
| **company_name** | varchar | NULL | default | Nombre de la empresa asociada al usuario o entidad[cite: 2]. |
| **email** | varchar | N-N | default | Dirección de correo electrónico del usuario[cite: 2]. |
| **first_name** | varchar | N-N | default | Primer nombre del usuario[cite: 2]. |
| **last_name** | varchar | N-N | default | Apellido del usuario[cite: 2]. |
| **password** | varchar | N-N | default | Contraseña del usuario (almacenada de forma segura, usualmente encriptada)[cite: 2]. |
| **trial** | bit | NULL | default | Indica si el usuario está en un período de prueba (true/false)[cite: 2]. |
| **username** | varchar | N-N | default | Nombre de usuario único utilizado para iniciar sesión[cite: 2]. |

**Tabla: USER_AUDITS**

| Campo | Tipo | Nulo | Default | Comentario / Descripción |
| :--- | :--- | :--- | :--- | :--- |
| **id** | bigint | N-N | default | Identificador único del registro de auditoría. |
| **user_id** | bigint | N-N | default | Clave foránea que referencia a la tabla USERS. |
| **action** | varchar | N-N | default | Descripción de la acción o evento realizado por el usuario. |
| **timestamp** | datetime | N-N | default | Fecha y hora exacta en la que se registró el evento de auditoría. |

