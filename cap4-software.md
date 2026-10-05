# 4 Product Implementation, Validation & Deployment

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

**Landing Page — GitHub Pages**

Enlace de despliegue: 

![Landing Page desplegada en Github deployment]()

**Landing Page — Repositorio GitHub**

Enlace del repositorio: https://github.com/BL-Aplicaciones-Web-1ASI0730-2610-12158/Vantage-PMO-Business-Web-Page

![Repositorio GitHub — Landing Page](assets/images/chapter-5/landing-page/landing-page-repository.png)

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

Repositorio de Código Fuente

Se debe crear un repositorio en GitHub y subir todos los archivos del proyecto (HTML, CSS, JS). Es obligatorio que el archivo index.html esté ubicado en la raíz del repositorio para poder realizar el despliegue correctamente.

![Github Repository](assets/images/chapter-5/landing-page/landing-page-repository.png)

## 4.2.1. Sprint 1
### 4.2.1.1. Sprint Planning 1
### 4.2.1.2. Aspect Leaders and Collaborators
### 4.2.1.3. Sprint Backlog 1

### 4.2.1.4. Development Evidence for Sprint Review

Durante el Sprint 1 se realizaron avances en la implementación de los productos que conforman Vantage PMO. Como parte del desarrollo, se avanzó en la construcción de los servicios del backend, incorporando la estructura necesaria para gestionar las principales capacidades del dominio mediante servicios RESTful.

El código fuente se mantiene en repositorios de GitHub, utilizando control de versiones para registrar los cambios realizados durante la implementación. En el backend se incorporaron componentes correspondientes a las capas de dominio, aplicación, infraestructura e interfaces REST, permitiendo establecer la base para las funcionalidades definidas para el Sprint 1.

A continuación, se presentan los commits asociados a los avances de implementación realizados durante el Sprint.

| Repository | Branch | Commit Id | Commit Message | Commit Message Body | Commited on (Date) |
| :--- | :--- | :--- | :--- | :--- | :--- |
| [MDEPS-Team/MDEPS-Back-End](https://github.com/MDEPS-Team/MDEPS-Back-End) | main | 062e857 | feat: backend migration | — | 2026-10-04 |

El commit presentado corresponde a la incorporación de la implementación inicial del backend de Vantage PMO, incluyendo la estructura de los diferentes módulos del dominio y los servicios REST necesarios para exponer las funcionalidades del sistema.

### 4.2.1.5. Testing Suite Evidence for Sprint Review

Durante el Sprint 1 se implementó una suite de pruebas automatizadas para validar parte de las funcionalidades del backend de Vantage PMO. Las pruebas fueron desarrolladas utilizando **xUnit** sobre **.NET 10**, incorporando pruebas unitarias, una prueba de integración y una prueba de aceptación bajo el enfoque BDD.

Las pruebas realizadas se encuentran relacionadas principalmente con la **US11 - Consultar indicadores de desempeño**, debido a que validan componentes pertenecientes al bounded context de Analytics, encargado de gestionar y proporcionar información relacionada con los indicadores de desempeño del portafolio.

La suite desarrollada permitió verificar tanto el comportamiento de objetos individuales del dominio como la interacción entre componentes de persistencia y la correcta satisfacción de un escenario de aceptación definido mediante Gherkin.

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

### 4.2.1.6. Execution Evidence for Sprint Review

Durante el Sprint 1 se avanzó en la implementación del backend de Vantage PMO, incluyendo la construcción de bounded contexts, servicios de aplicación, repositorios, controladores REST y configuración de persistencia.

Como parte del trabajo realizado durante el Sprint, se implementaron componentes correspondientes a módulos como Analytics, Projects, Dashboard, Meetings, Profiles, Reports, Resource Planning, Risk Compliance, Schedule, Settings, Support, Task Collaboration y Workspace.

Asimismo, se configuró la exposición de servicios mediante controladores REST y documentación OpenAPI/Swagger, estableciendo los endpoints necesarios para las funcionalidades desarrolladas en el backend.

Durante la validación técnica del Sprint se comprobó que el proyecto compila correctamente y que la suite de pruebas automatizadas implementada para el módulo Analytics finaliza satisfactoriamente. Las pruebas realizadas incluyen dos pruebas unitarias, una prueba de integración y una prueba de aceptación bajo BDD, todas ejecutadas correctamente.

Estos resultados evidencian el avance alcanzado en la implementación técnica del backend durante el Sprint 1 y proporcionan una base para la integración posterior con las interfaces de usuario y los flujos funcionales del producto.

### 4.2.1.7. Services Documentation Evidence for Sprint Review
### 4.2.1.8. Software Deployment Evidence for Sprint Review
### 4.2.1.9. Team Collaboration Insights during Sprint
