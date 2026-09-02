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

### 2.6.1. Bounded Context: [Nombre del Bounded Context 1]
#### 2.6.1.1. Domain Layer
[Aggregates, Entities, Value Objects, Commands, Queries, Services e Interfaces].

#### 2.6.1.2. Interface Layer
[Controllers, Resources/DTOs, Assemblers].

#### 2.6.1.3. Application Layer
[Command Handlers, Query Handlers, Outbound Services].

#### 2.6.1.4. Infrastructure Layer
[Repositories concretos, persistencia, adaptadores externos].

#### 2.6.1.5. Bounded Context Software Architecture Component Level Diagrams
[Diagrama C4 Nivel 3 de Componentes].

#### 2.6.1.6. Bounded Context Software Architecture Code Level Diagrams
##### 2.6.1.6.1. Bounded Context Domain Layer Class Diagrams
[Diagrama UML de clases del dominio].

##### 2.6.1.6.2. Bounded Context Database Design Diagram
[Diagrama de base de datos relacional y diccionario de tablas].