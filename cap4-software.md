<div style="page-break-before: always;"></div>

# IV Product Implementation, Validation & Deployment

## 4.1. Software Configuration Management
<a id="5-1-software-configuration-management"></a>

### 4.1.1. Software Development Environment Configuration
<a id="5-1-1-software-development-environment-configuration"></a>

A continuación, se listan las herramientas y estándares adoptados por el equipo para el desarrollo colaborativo del sistema:

| Actividad               | Herramienta / Guía | Propósito                                                                    | Tipo de acceso / Ruta     |
| ----------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Project Management      | Trello Software   | Seguimiento de backlog, tareas y sprints.                                     | SaaS –[https://trello.com/](https://trello.com/software/jira)          |
| Requirements Management | Gherkin Conventions   | Escritura legible de requisitos con formato Given/When/Then.                  | [https://cucumber.io/docs/gherkin/](https://cucumber.io/docs/gherkin/)          |
| Product UX/UI Design    | Figma   | Prototipos y diseño responsive.                                              | SaaS –[https://figma.com](https://figma.com)     |
| Landing Page             | HTML, CSS, JavaScript, Vue     | Construcción de la interfaz web.                                             | [https://vuejs.org/guide/introduction.html](https://vuejs.org/guide/introduction.html)       |
| User Personas, Empathy Journey Mapping, Impact Mapping   | UXPressia                | Es una herramienta en línea para el mapeo de la trayectoria del cliente que crea mapas de impacto y personas.    | [https://uxpressia.com/](https://uxpressia.com/)        |
| Class Diagram and Database Diagram  | LucidChart | Organización y modelado de las tablas y entidades del proyecto.         | [https://www.lucidchart.com/](https://www.lucidchart.com/)                                                                            |
| Code Standards          | Google HTML/CSS Style Guide, Vue Style Guide, MDN Guidelines, W3C JavaScript Style Guide, Google JavaScript Style Guide, C# Coding Conventions, Microsoft ASP.NET Core Guidelines | Aplicación de buenas prácticas de desarrollo en frontend y backend.         | [https://developer.mozilla.org/](https://developer.mozilla.org/) / [https://learn.microsoft.com/en-us/dotnet/csharp/fundamentals/coding-style](https://learn.microsoft.com/en-us/dotnet/csharp/fundamentals/coding-style) |
| Version Control         | Git + GitHub     | Control de versiones y trabajo colaborativo.                                  | SaaS –[https://github.com](https://github.com)  |
| Software Deployment     | Github pages   | Despliegue continuo de la aplicación para ambientes de prueba y validación. | SaaS –[https://railway.app](https://railway.app) / [https://render.com](https://render.com)  |
| Upgrade of Branches and Commits | Visual Studio Code | Optimización y documentación del proyecto asimismo el trabajo colaborativo. |[https://code.visualstudio.com/](https://code.visualstudio.com/)  |
| EventStorming | Miro | Herramienta colaborativa grupal que permitio diseñar mejor algunos puntos del trabajo. |[https://miro.com/es/](https://miro.com/es/)  |

<div style="text-align: left; max-width: 900px; margin: 0 auto;">

### 4.1.2. Source Code Management
<a id="5-1-2-source-code-management"></a>

Para la gestión del código del proyecto, el equipo adoptó una estrategia simplificada en lugar de implementar completamente el modelo Git Flow. Se trabajó principalmente sobre una rama principal (main), la cual contiene la versión estable y actual del sistema en desarrollo. 

Adicionalmente, se crearon algunas ramas específicas organizadas por capítulos del proyecto. Estas ramas permitieron desarrollar avances de manera más ordenada antes de integrarlos a la rama principal, sin llegar a una estructura compleja de múltiples ramas por funcionalidades o versiones. 

Todas las funcionalidades y mejoras fueron finalmente integradas en la rama main, asegurando que esta siempre represente el estado más actualizado del proyecto. Este enfoque, aunque más sencillo que Git Flow, resultó adecuado para el alcance del trabajo, ya que facilitó el control del progreso sin generar una sobrecarga en la gestión de ramas.

 Por otro lado, se utilizó GitHub como repositorio central del proyecto, aprovechando también herramientas como GitHub Pages para la visualización del Landing Page. Esto permitió desplegar rápidamente los avances en formato web y contar con una versión accesible del sistema de manera ágil y eficiente.

---

URL de los Repositorios:
Organización: https://github.com/MDEPS-Team
Reporte: https://github.com/MDEPS-Team/MDEPS-Landing-page
Landing Page: https://github.com/MDEPS-Team/MDEPS-Landing-page
Backend: https://github.com/MDEPS-Team/MDEPS-Back-End


### Versionado Semántico

Se aplicará el esquema de **Semantic Versioning 2.0.0**, con el siguiente formato:

- **MAJOR**: Incompatibilidades en la API.
- **MINOR**: Nuevas funcionalidades sin romper compatibilidad.
- **PATCH**: Correcciones de errores menores y ajustes sin afectar funcionalidades.

_Ejemplo de versión:_ `v1.3.4`

### Convenciones de Commits

Se adoptará el estándar de **Conventional Commits** para la redacción de los mensajes de commit, lo cual permitirá estructurar mejor los cambios realizados. Este enfoque facilita la automatización de procesos como la integración continua y la generación de historiales de cambios (changelogs).

**Ejemplos:**

- `feat: add project creation form`
- `fix: resolve error in task assignment module`
- `docs: update user stories and diagrams`
- `chore: update dependencies`
### 4.1.3. Source Code Style Guide & Conventions
<a id="5-1-3-source-code-style-guide-conventions"></a>

El código desarrollado por los miembros del equipo esté completamente redactado en inglés.

## **HTML**

* **Use Lowercase Element Names**: Se recomienda utilizar minúsculas para todos los elementos HTML.
```html
<section class="hero">
<h1>Centralize your projects</h1>
</section>

**Close All HTML Elements**: Todos los elementos deben cerrarse correctamente para evitar errores de renderizado.
```html
<p>Centralize your projects, control your future.</p>

<a href="#Contact">Solicitar demo</a>
```

**Use Lowercase Attribute Names**: Los atributos deben escribirse en minúsculas.

```html
<input type="email" placeholder="tu@correo.com" id="fe"/>
```
**Use Semantic HTML Elements**: Se deben utilizar etiquetas semánticas para mejorar la estructura y accesibilidad.

```html
<nav>...</nav>
<section id="funciones">...</section>
<footer>...</footer>
```

**Use Descriptive IDs and Classes**: Los nombres deben ser claros y representar su función.
```html
<section id="contact">
  <div class="contact-form">
```
## **CSS**

**Use Kebab-Case for Class Names**: Las clases deben escribirse en minúsculas separadas por guiones.
```css
.contact-form {
  display: flex;
}
```
**Use CSS Variables for Colors**: Se deben definir colores reutilizables en :root.
```css
:root {
  --blue: #1E40AF;
  --navy: #0F172A;
}
```
**Group Styles by Sections**: El código CSS debe organizarse por secciones del sitio.
```css
/* NAV */
nav { ... }
/* HERO */
.hero { ... }
/* FOOTER */
footer { ... }
```
**Use Consistent Spacing**: Se debe mantener consistencia en márgenes, padding y alineación.
```css
.section {
  padding: 6rem 2rem;
}
```
**Responsive Design with Media Queries**: Se deben usar breakpoints para adaptar la interfaz.
```css
@media (max-width: 600px) {
  .hero {
    padding: 4rem 1rem;
  }
}
```
## **JavaScript**

**Use CamelCase for Variables and Functions**: Las variables y funciones deben usar camelCase.
```js
function sendForm() {
  const userName = document.getElementById('fn').value;
}
```
**Keep Functions Simple and Clear**: Las funciones deben ser cortas y fáciles de entender.
```js
if (!n || !e) {
  alert('Por favor completa tu nombre y correo.');
  return;
}
```

**Use Meaningful Variable Names**: Los nombres deben representar su propósito.
```js
const navLinks = document.getElementById('navLinks');
const hamburger = document.getElementById('hamburger');
```
**Avoid Inline JavaScript**: Se recomienda mantener la lógica separada del HTML.
```js
< button onclick="sendForm()">Enviar</ button>
```
### 4.1.4. Software Deployment Configuration
<a id="5-1-4-software-deployment-configuration"></a>

Para la Landing Page desarrollada en HTML, CSS y JavaScript, la configuración del despliegue en GitHub Pages se define de la siguiente manera:

**Repositorio de Código Fuente**

Se debe crear un repositorio en GitHub y subir todos los archivos del proyecto (HTML, CSS, JS). Es obligatorio que el archivo index.html esté ubicado en la raíz del repositorio para poder realizar el despliegue correctamente.

![img.png](img.png)

**Despliegue del Backend (Web Service)**

Para el despliegue de la API REST y la base de datos, se utilizó la plataforma **Railway**. El proceso de configuración consistió en:
1. Provisión de un servicio de base de datos **MySQL** alojado en la nube.
2. Vinculación directa con el repositorio de GitHub (`MDEPS-Back-End`) utilizando el archivo `Dockerfile` ubicado en la raíz del proyecto para la compilación del entorno en .NET 10.
3. Configuración de variables de entorno, incluyendo la cadena de conexión a la base de datos (`ConnectionStrings__DefaultConnection`) y la habilitación de la documentación pública (`ASPNETCORE_ENVIRONMENT = Development`).
## 4.2. Sprint Development, Planning and Execution

La implementación de Vantage PMO se organiza en tres sprints hasta la entrega del Trabajo Final. La planificación parte del Product Backlog definido en la sección 2.4.3 y distribuye las 17 User Stories según sus dependencias, esfuerzo relativo y entregables previstos. Los periodos se presentan por semanas académicas, conforme a la planificación consignada por el equipo.

| Sprint | Periodo planificado | Objetivo del sprint | User Stories | Story Points | Entregables previstos |
| :---: | :--- | :--- | :--- | :---: | :--- |
| **Sprint 1** | Semanas 4 a 7 | Definir la experiencia de usuario y establecer la base técnica y operativa de la solución. | US16, US17, US01, US02, US03, US04, US05 | **24** | Wireframes, Mock-ups y prototipo móvil; User Flows; Landing Page desplegada; avance de servicios backend y evidencia de las pantallas core. |
| **Sprint 2** | Semanas 8 a 12 | Ampliar las capacidades operativas de control y análisis de los proyectos. | US07, US09, US11, US13, US12 | **28** | Gestión de riesgos y documentos; indicadores y reportes; alertas; integración progresiva con los servicios backend y aplicación móvil. |
| **Sprint 3** | Semanas 13 a 15 | Completar las funcionalidades avanzadas y validar la solución integrada para su presentación final. | US15, US08, US06, US14, US10 | **26** | Gestión avanzada de roles; asignación de recursos; comunicación de bloqueos; consulta de proyectos desde móvil; captura de evidencias y pruebas finales de integración. |
| **Total** | Semanas 4 a 15 | Implementar y validar el alcance definido para Vantage PMO. | **17 User Stories** | **78** | **Alcance acumulado de los tres sprints.** |

El Sprint 1 corresponde a la primera entrega de diseño e implementación y recoge el avance del backend indicado para la TB1. Los entregables de los sprints 2 y 3 representan objetivos planificados, no funcionalidades que se declaren concluidas anticipadamente. Para el seguimiento se utiliza Trello, donde cada historia debe estar vinculada al sprint correspondiente y a las tareas que permiten producir sus evidencias.

La aceptación de una User Story requiere comprobar sus criterios de aceptación, además del registro de las tareas relacionadas. Por tanto, los Story Points planificados no deben confundirse con la velocidad real del equipo, que depende exclusivamente de las historias aceptadas al cierre de cada sprint.

### 4.2.1. Sprint 1
#### 4.2.1.1. Sprint Planning 1

El Sprint Planning 1 estableció el alcance inicial de Vantage PMO para las semanas 4 a 7. Se priorizó la construcción de los artefactos de diseño, la definición de los recorridos principales de la aplicación, el despliegue de la Landing Page y el avance inicial del backend. Las historias incluidas se seleccionaron a partir del Product Backlog y de sus dependencias funcionales.

| Campo | Detalle |
| :--- | :--- |
| **Sprint #** | Sprint 1 |
| **Periodo planificado** | Semanas 4 a 7 |
| **Date** | 20 de septiembre de 2026 |
| **Time** | 10:00 a. m. |
| **Location** | Reunión virtual mediante Microsoft Teams |
| **Prepared By** | Fuentes Alvarez, Angiela Stephany |
| **Attendees** | Fuentes Alvarez, Angiela Stephany; Guillen Giraldo, Mike Dylan; Mendoza Machoa, Lionel Snayder; Pacheco Lavado, Rafael Agustin; Quiliano Motta, Kirk Douglas |
| **Sprint n-1 Review Summary** | No aplica: es el primer sprint. |
| **Sprint n-1 Retrospective Summary** | No aplica: es el primer sprint. |
| **Sprint Goal** | Establecer la propuesta visual y los flujos de interacción de Vantage PMO, junto con la infraestructura técnica necesaria para las primeras operaciones sobre proyectos y tareas. |
| **User Stories planificadas** | US16, US17, US01, US02, US03, US04, US05. |
| **Story Points comprometidos en la planificación** | **24 Story Points.** |
| **Sprint 1 Velocity (real)** | Se determina según las historias que cumplieron sus criterios de aceptación al cierre del sprint; no equivale automáticamente a los 24 puntos planificados. |

**Entregables asociados al Sprint 1:**

- **Landing Page:** wireframes, mock-ups, implementación y evidencia del despliegue, alineados con US16 y US17.
- **Experiencia móvil:** wireframes, mock-ups, wireflows, User Flows de los procesos principales y prototipo navegable.
- **Gestión de proyectos y tareas:** diseño y avance técnico de las funciones de registro de proyectos, fases, consulta del portafolio y asignación/seguimiento de tareas (US01 a US05, según corresponda).
- **Backend:** evidencia del avance presentado en TB1, repositorio y servicios desarrollados; el porcentaje declarado debe sustentarse con funcionalidades y pruebas comprobables.
- **Control del trabajo:** backlog en Trello, asignación de responsables, registro de tareas y evidencias relacionadas con la ejecución.

Esta planificación distingue el alcance funcional esperado de las actividades de diseño y de las evidencias técnicas. La existencia de un mock-up o un prototipo no se considera, por sí sola, demostración de que toda la funcionalidad de una User Story esté implementada y aceptada.

#### 4.2.1.2. Aspect Leaders and Collaborators

En el marco del Sprint 1, se han priorizado las actividades relacionadas con la transformación de los requerimientos y hallazgos obtenidos durante las etapas de análisis en propuestas concretas de diseño y planificación para Vantage PMO. Los esfuerzos del equipo se orientan hacia el diseño de la Landing Page, el diseño UX/UI de la aplicación móvil, la elaboración de flujos de usuario y prototipos, así como las actividades relacionadas con la implementación y documentación de la solución.

A fin de garantizar una ejecución coordinada y una adecuada distribución de responsabilidades, se ha implementado la Matriz de Liderazgo y Colaboración (LACX). En esta herramienta se identifican los responsables principales (L) y los colaboradores (C) para cada aspecto del Sprint 1.

| **Team Member (Last Name, First Name)** | **GitHub Username** | **Landing Page** | **Mobile App UX/UI** | **User Flows & Prototyping** | **Implementation** | **Testing** | **Documentation** |
| :--- | :--- | :---: | :---: | :---: | :---: | :---: | :---: |
| Fuentes Alvarez, Angiela Stephany | angielafuentes | L | C | C | C | C | L |
| Guillen Giraldo, Mike Dylan | mikeguillen | C | L | C | C | C | C |
| Mendoza Machoa, Lionel Snayder | mendozalionel745-ctrl | C | C | L | L | C | C |
| Pacheco Lavado, Rafael Agustin | RafaelAgustin21 | C | C | C | C | L | C |
| Quiliano Motta, Kirk Douglas | Kirkelto | C | C | C | C | C | L |


#### 4.2.1.3. Sprint Backlog 1

El Sprint Backlog 1 detalla los work-items documentados para materializar los entregables del primer sprint. Los ítems se vinculan con las User Stories correspondientes y abarcan diseño de la Landing Page, diseño móvil, representación de flujos, prototipado y configuración inicial del backend.

La Landing Page atiende dos historias complementarias: US16, referida a la presentación de la propuesta de valor, y US17, centrada en los medios de contacto. Por ello, ambas se relacionan con las actividades de diseño general T001 y T002; esta asociación debe mantenerse también en Trello. Los estados y estimaciones de la siguiente tabla se reproducen a partir del registro de trabajo del equipo y deben contrastarse con el tablero antes de la entrega.

**Evidencia del tablero de trabajo**

![Sprint Backlog 1 en Trello](assets/images/chapter-4/sprint-backlog/sprint-backlog-01.png)

| User Story | Work-item | Tarea | Descripción | Estimación (h) | Responsable | Estado documentado |
| :--- | :---: | :--- | :--- | ---: | :--- | :---: |
| US16, US17 | T001 | Elaborar wireframes de la Landing Page | Organizar la propuesta de valor, las áreas de contenido y los puntos de acceso a contacto. | 3 | Angiela Fuentes | Done |
| US16, US17 | T002 | Elaborar mock-ups de la Landing Page | Aplicar la identidad visual definida a las secciones informativas y de contacto. | 4 | Angiela Fuentes | Done |
| US01 | T003 | Elaborar wireframes de la aplicación | Diseñar las vistas asociadas al registro de proyectos. | 4 | Mike Guillen | Done |
| US01 | T004 | Configurar la base del backend | Establecer la estructura inicial en .NET para las capacidades de proyectos. | 6 | Lionel Mendoza | Done |
| US02 | T005 | Elaborar mock-ups de proyectos e hitos | Representar la gestión de proyectos, fases e hitos en la interfaz móvil. | 5 | Mike Guillen | Done |
| US03 | T006 | Elaborar Wireflow Diagrams | Describir la navegación de consulta del portafolio, vinculada con UG-03. | 4 | Lionel Mendoza | Done |
| US03 | T007 | Elaborar User Flow Diagrams | Representar el recorrido de consulta del portafolio y sus decisiones. | 5 | Lionel Mendoza | Done |
| US04 | T008 | Diseñar Kanban y asignación de tareas | Crear wireframes y mock-ups del tablero y de la asignación de responsables. | 4 | Mike Guillen | Done |
| US05 | T009 | Integrar el prototipo de tareas | Incorporar las vistas de Kanban y los cambios de estado al prototipo navegable. | 3 | Lionel Mendoza | Done |
| **Total** | **9 tareas** | | | **38 h** | | |

Las 38 horas corresponden a la suma de las estimaciones de tareas documentadas; no deben compararse directamente con los 24 Story Points del sprint, ya que se trata de unidades diferentes. Los nueve work-items representan actividades de avance y no necesariamente la totalidad de las tareas de implementación necesarias para aceptar las siete historias planificadas.

**Control de consistencia:** el tablero de Trello debe mostrar explícitamente los tres sprints y mantener la correspondencia entre identificadores de User Story, responsables, tareas y estados. Asimismo, las correcciones de User Flows solicitadas en el feedback deben registrarse como trabajo de mejora, sin modificar retroactivamente el estado histórico de las actividades de diseño completadas.

#### 4.2.1.4. Development Evidence for Sprint Review

Durante el Sprint 1 se realizaron avances en la implementación de los productos que conforman Vantage PMO. Como parte del desarrollo, se avanzó en la construcción de los servicios del backend, incorporando la estructura necesaria para gestionar las principales capacidades del dominio mediante servicios RESTful.

El código fuente se mantiene en repositorios de GitHub, utilizando control de versiones para registrar los cambios realizados durante la implementación. En el backend se incorporaron componentes correspondientes a las capas de dominio, aplicación, infraestructura e interfaces REST, permitiendo establecer la base para las funcionalidades definidas para el Sprint 1.

A continuación, se presentan los commits asociados a los avances de implementación realizados durante el Sprint.

| Repository | Branch | Commit Id | Commit Message | Commit Message Body | Commited on (Date) |
| :--- | :--- | :--- | :--- | :--- | :--- |
| [MDEPS-Team/MDEPS-Back-End](https://github.com/MDEPS-Team/MDEPS-Back-End) | main | 062e857 | feat: backend migration | — | 2026-10-04 |

El commit presentado corresponde a la incorporación de la implementación inicial del backend de Vantage PMO, incluyendo la estructura de los diferentes módulos del dominio y los servicios REST necesarios para exponer las funcionalidades del sistema.

#### 4.2.1.5. Testing Suite Evidence for Sprint Review

Durante el Sprint 1, el equipo documentó una suite inicial de pruebas automatizadas del backend de Vantage PMO utilizando xUnit sobre .NET 10. Esta suite comprende pruebas unitarias, una prueba de integración con Entity Framework Core InMemory y una prueba de aceptación expresada mediante Gherkin.

Aunque el alcance funcional planificado para el Sprint 1 corresponde a US16, US17 y US01–US05, las pruebas registradas en esta sección están vinculadas a **US11 — Consultar indicadores de desempeño**, historia prevista para el Sprint 2. Esto se consigna como **trabajo técnico anticipado sobre el bounded context Analytics** y no como evidencia de que US11 haya sido completada o aceptada en el Sprint 1.

Los resultados de estas pruebas sirven para verificar componentes iniciales del dominio y de persistencia utilizados por Analytics. La aceptación de US11 y su contabilización como Story Points completados deben revisarse dentro del sprint al que fue asignada, con evidencia de que se satisfacen sus criterios de aceptación funcional.

#### Unit Tests

Para las pruebas unitarias se seleccionaron objetos de valor pertenecientes al módulo Analytics. El objetivo fue comprobar que los objetos mantengan correctamente la información proporcionada durante su creación.

| Test ID | Test Type | Related User Story | Class | Test | Description |
| :--- | :--- | :--- | :--- | :--- | :--- |
| UT01 | Unit Test | US11 | `SummaryKpis` | `Constructor_ShouldAssignProvidedValues` | Verifica que los valores correspondientes a fondos disponibles, índice de velocidad, exposición al riesgo y planes de mitigación sean asignados correctamente al crear un objeto `SummaryKpis`. |
| UT02 | Unit Test | US11 | `PortfolioRoi` | `Constructor_ShouldAssignProvidedValues` | Verifica que el porcentaje de ROI, nivel de eficiencia, valor objetivo y valor proyectado sean almacenados correctamente en un objeto `PortfolioRoi`. |

Estas pruebas permiten validar de manera aislada los objetos utilizados para representar los principales indicadores de desempeño mostrados por el módulo Analytics.

#### Integration Tests

Para validar la interacción entre la capa de persistencia y el dominio se implementó una prueba de integración utilizando **Entity Framework Core InMemory**.

| Test ID | Test Type | Related User Story | Component | Test | Description |
| :--- | :--- | :--- | :--- | :--- | :--- |
| IT01 | Integration Test | US11 | `AnalyticsDashboardRepository` | `AddAndList_ShouldPersistAndReturnAnalyticsDashboard` | Verifica que un objeto `AnalyticsDashboard` pueda almacenarse mediante el repositorio y posteriormente recuperarse correctamente, conservando sus indicadores y datos asociados. |

La prueba utiliza una base de datos en memoria para verificar la integración entre `AppDbContext`, Entity Framework Core y `AnalyticsDashboardRepository`, evitando modificar la base de datos utilizada por la aplicación durante el desarrollo.

#### Acceptance Tests

Para validar el comportamiento esperado desde la perspectiva del usuario se implementó un Acceptance Test bajo el enfoque **Behavior-Driven Development (BDD)**.

El escenario se relaciona con la **US11 - Consultar indicadores de desempeño**, donde el Project Manager debe poder consultar los indicadores correspondientes al desempeño del portafolio.

El escenario fue definido mediante un archivo `.feature` utilizando Gherkin:

```gherkin
Feature: Analytics Dashboard

  As a Project Manager
  I want to consult portfolio performance indicators
  So that I can identify the current state and performance of the projects

  Scenario: Consult portfolio performance indicators successfully
    Given that analytics information exists for the portfolio
    When the Project Manager requests the analytics dashboard
    Then the system returns the portfolio performance indicators
```

Los Steps correspondientes fueron implementados en la clase `AnalyticsDashboardSteps`. En el paso `Given` se prepara información de Analytics utilizando una base de datos en memoria; en el paso `When` se consulta la información mediante `AnalyticsDashboardRepository`; finalmente, en el paso `Then` se verifica que el sistema retorne correctamente los indicadores de desempeño esperados.

| Test ID | Test Type | Related User Story | Feature | Scenario |
| :--- | :--- | :--- | :--- | :--- |
| AT01 | Acceptance Test - BDD | US11 | Analytics Dashboard | Consult portfolio performance indicators successfully |

#### Testing Execution Evidence

La ejecución de la suite de pruebas fue realizada mediante el Test Explorer de Visual Studio. Como resultado se ejecutaron cuatro pruebas automatizadas, obteniendo los siguientes resultados:

| Test Type | Tests Executed | Passed | Failed |
| :--- | :---: | :---: | :---: |
| Unit Tests | 2 | 2 | 0 |
| Integration Tests | 1 | 1 | 0 |
| Acceptance Tests | 1 | 1 | 0 |
| **Total** | **4** | **4** | **0** |

La ejecución confirmó que las cuatro pruebas implementadas finalizaron correctamente, sin presentar errores ni pruebas omitidas.

![Testing Suite Execution - Sprint 1](assets/images/chapter-4/testing/testing-suite-sprint-1.png)

*Figura. Ejecución de la suite de pruebas del backend de Vantage PMO en Visual Studio, mostrando cuatro pruebas superadas y cero errores.*

Asimismo, la siguiente evidencia muestra el escenario de aceptación definido mediante Gherkin para la consulta de indicadores de desempeño.

![Analytics Dashboard Feature](assets/images/chapter-4/testing/analytics-dashboard-feature.png)

*Figura. Escenario de Acceptance Test en Gherkin correspondiente a la US11 - Consultar indicadores de desempeño.*

#### Testing Repository and Commits

Los archivos correspondientes a las pruebas automatizadas se encuentran almacenados dentro del repositorio del backend de Vantage PMO, en el proyecto `vantagePMO-platform.Tests`.

**Repository:** [MDEPS-Team/MDEPS-Back-End](https://github.com/MDEPS-Team/MDEPS-Back-End)

Los principales archivos incorporados para la suite de pruebas son:

- `vantagePMO-platform.Tests/SummaryKpisTests.cs`
- `vantagePMO-platform.Tests/PortfolioRoiTests.cs`
- `vantagePMO-platform.Tests/AnalyticsDashboardRepositoryIntegrationTests.cs`
- `vantagePMO-platform.Tests/Features/analytics-dashboard.feature`
- `vantagePMO-platform.Tests/Features/Steps/AnalyticsDashboardSteps.cs`
- `vantagePMO-platform.Tests/vantagePMO-platform.Tests.csproj`

A continuación, se presenta el commit relacionado con la implementación de las pruebas durante el Sprint 1.

| Repository | Branch | Commit Id | Commit Message | Commit Message Body | Commited on (Date) |
| :--- | :--- | :--- | :--- | :--- | :--- |
| MDEPS-Team/MDEPS-Back-End | feature/4.2.1.5-testing | ff70649 | test: add sprint 1 backend test suite | — | 2026-10-05 |

#### 4.2.1.6. Execution Evidence for Sprint Review
<a id="5-2-1-5-execution-evidence-for-sprint-review"></a>

Durante el presente Sprint, se ha logrado la transición de una interfaz estática a un ecosistema interactivo y funcional, cumpliendo con el objetivo de establecer el núcleo de acceso y la propuesta de valor visual de Vantage PMO. Los hitos alcanzados se centran en la implementación de un sistema de seguridad robusto, la personalización dinámica de la identidad de marca y la optimización de la experiencia de usuario a través de múltiples dispositivos y lenguajes.

**Resumen de Logros:**

- Seguridad y Acceso: Se ha desplegado un módulo de autenticación completo que integra proveedores de identidad modernos, garantizando un flujo de inicio de sesión seguro, validado y alineado con normativas legales de privacidad.

- Interactividad y Demostración: Se implementó un motor de previsualización en tiempo real que permite a los potenciales clientes interactuar con la plataforma, personalizando elementos de branding y visualizando la capacidad del dashboard de portafolio sin fricciones técnicas.

- Accesibilidad y Alcance Global: Gracias a la implementación de internacionalización (i18n) y un diseño estrictamente responsivo, la plataforma es ahora capaz de ofrecer una navegación coherente y profesional tanto en entornos de escritorio como en dispositivos móviles, eliminando barreras de idioma y formato.

- Comunicación Persistente: Se estableció la infraestructura de notificaciones push, permitiendo una conexión directa con el usuario y mejorando los índices de retención mediante alertas del sistema optimizadas.

A continuación, se presentan las evidencias gráficas de las vistas implementadas y el recurso audiovisual que detalla el flujo de navegación alcanzado:

Video de Demostración y Navegación: https://upcedupe-my.sharepoint.com/:v:/g/personal/u202417433_upc_edu_pe/IQBngnzzXajyRpPAik2w-PdQAW6q0V01RTT5qhqPQLRNLcg?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=SXvFNG

Screenshots de la Implementación:

![img_1.png](assets/images/img_1.png)

**Ejecución e Interactividad del Backend**

Además del entorno web, se logró desplegar exitosamente el backend de Vantage PMO basado en arquitectura DDD y CQRS. A través de la interfaz interactiva de Swagger, se demostró la ejecución real de los Endpoints de los distintos Bounded Contexts (Authentication, Projects, Analytics, etc.).

Durante la validación, se ejecutaron peticiones `POST` para la creación de entidades y peticiones `GET` para verificar su correcta persistencia en la base de datos MySQL alojada en Railway, confirmando que la API no retorna datos simulados, sino que procesa transacciones reales.

![img.png](assets/img5.png)
*Figura: Interfaz interactiva de Swagger documentando los Bounded Contexts del sistema.*

![img.png](assets/img7.png)
*Figura: Ejecución de un endpoint de la API y respuesta HTTP validando la persistencia en la base de datos.*

#### 4.2.1.7. Services Documentation Evidence for Sprint Review
#### 4.2.1.8. Software Deployment Evidence for Sprint Review
#### 4.2.1.9. Team Collaboration Insights during Sprint
