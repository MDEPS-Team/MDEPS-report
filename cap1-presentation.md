# Capitulo I: Presentacion

## 1.1. Startup Profile

### 1.1.1. Descripcion de la Startup
Somos una startup peruana denominada **MDEPS** (Managements Development Engineering Project Systems), creada por estudiantes de la carrera de Ingeniería de Software de la Universidad Peruana de Ciencias Aplicadas (UPC), que tiene como objetivo principal optimizar la gestión de proyectos dentro de las organizaciones mediante el uso de tecnología.

Nuestra misión es lograr que ninguna empresa gestione sus proyectos sin un control centralizado, estandarizado y basado en información confiable, reduciendo así problemas como retrasos, falta de visibilidad, mala comunicación y toma de decisiones ineficientes.

Para cumplir con este propósito, hemos desarrollado el proyecto **MDEPS** (Project Management Office), una plataforma movil que permite a las organizaciones gestionar, monitorear y controlar todos sus proyectos de manera centralizada, brindando visibilidad en tiempo real, estandarización de procesos y herramientas inteligentes para la toma de decisiones.

### 1.1.2. Perfiles de integrantes del equipo
- **Fuentes Alvarez, Angiela Stephany**  
  [Foto]  
  *Codigo:*   | *Carrera:* Ingenieria de Software  
  *Resumen:* [].

- **Guillen Giraldo, Mike Dylan**  
  [Foto]  
  *Codigo:* [Codigo] | *Carrera:* Ingenieria de Software  
  *Resumen:* [Habilidades tecnicas y aportes al equipo].

- **Mendoza Machoa, Lionel Snayder**  
  [Foto]  
  *Codigo:* [Codigo] | *Carrera:* Ingenieria de Software  
  *Resumen:* [Habilidades tecnicas y aportes al equipo].

- **Pacheco Lavado, Rafael Agustin**  
  [Foto]  
  *Codigo:* [Codigo] | *Carrera:* Ingenieria de Software  
  *Resumen:* [Habilidades tecnicas y aportes al equipo].

- **Quiliano Motta, Kirk Douglas**  
  ![Foto-Kirk](assets/images/Kirk.png)    
  *Codigo:* [u202411378 ] | *Carrera:* Ingenieria de Software  
  *Resumen:* [Estudiante de la carrera de Ing. Software cursando el 6to ciclo y entusiasmado por aprender lo mas que pueda con conocimientos en lenguajes como python,
  c++, javascript, html, css, etc.].

---

## 1.2. Solution Profile

### 1.2.1. Antecedentes y problematica
#### What / ¿QUÉ?
Se presenta una fragmentación de la información y falta de visibilidad en la ejecución de proyectos, lo que impide un control centralizado y eficiente de los recursos organizacionales.

#### When / ¿CUÁNDO?
El problema se manifiesta críticamente durante las reuniones de seguimiento, en la entrega de reportes mensuales de desempeño y al momento de asignar recursos a nuevos hitos del proyecto.

#### Where / ¿DÓNDE?
Se observa principalmente en los departamentos de gestión de proyectos (PMO) y áreas operativas de empresas medianas y grandes que manejan múltiples portafolios de forma simultánea.

#### Who / ¿QUIÉN?
Afecta a los Project Managers y Stakeholders encargados de la toma de decisiones, cuya gestión se ve limitada por el uso de herramientas aisladas. Por ejemplo, hojas de cálculo o software no integrado, etc.

#### Why / ¿POR QUÉ?
Sucede debido a la ausencia de un estándar tecnológico que unifique los datos, lo que genera silos de información, procesos manuales propensos al error y falta de comunicación en tiempo real.

#### How / ¿CÓMO?
A diferencia del estado óptimo, donde la información fluye automáticamente, el problema se presenta como un patrón de retrasos constantes y desalineación entre los objetivos estratégicos y los resultados operativos.

#### How Much / ¿CUÁNTO?
Las organizaciones pierden entre un 20% y 30% de su productividad semanal en tareas de recopilación manual de datos, lo que se traduce en sobrecostos operativos y posibles multas por incumplimiento de plazos.

**Objetivos del Proyecto:**
- Desarrollar un producto de software consistente en una aplicacion movil y plataforma de soporte (MDEPS) que centralice la gestion de portafolios y reduzca el tiempo de consolidacion de reportes mensuales en un 25%.
- Integrar un servicio RESTful de desarrollo interno y consumir servicios externos para garantizar la sincronizacion de datos en tiempo real entre los equipos operativos y la gerencia, facilitando la toma de decisiones.

**Restricciones:**
- El desarrollo completo de la solucion de software esta estrictamente limitado al periodo academico de 15 semanas, debiendo cumplir con las entregas programadas (AV1, TB1, AV2, TB2).
- La arquitectura y el control de versiones deben aplicar obligatoriamente las practicas exigidas: uso de GitFlow, Conventional Commits, Semantic Versioning y Domain-Driven Design (DDD).
- El alcance del Producto Minimo Viable (MVP) se centrara unicamente en las funcionalidades core de monitoreo, asignacion de recursos y reportes, excluyendo integraciones complejas con sistemas ERP heredados (como SAP u Oracle) debido a limitaciones de tiempo.

### 1.2.2. Lean UX Process

#### 1.2.2.1. Lean UX Problem Statements
El estado actual de la gestion de proyectos en organizaciones medianas y grandes se ha enfocado principalmente en procesos manuales, hojas de calculo aisladas y comunicacion fragmentada, lo que resulta en una perdida de productividad de hasta el 30%.

Lo que los productos o servicios existentes no logran abordar es la necesidad de una plataforma centralizada y estandarizada que permita a los Project Managers y Stakeholders alinear los objetivos estrategicos con los resultados operativos sin una curva de aprendizaje tecnica excesiva.

Nuestro producto o servicio abordara esta brecha mediante una plataforma web y movil (MDEPS) que automatice el control de hitos, proporcione visibilidad en tiempo real y unifique los datos para la toma de decisiones.

Nuestro enfoque inicial seran los Project Managers, PMO Leads y Stakeholders de empresas medianas y grandes.

Sabremos que tenemos exito cuando veamos una reduccion del 25% en el tiempo de elaboracion de reportes, una disminucion en los sobrecostos por retrasos y un incremento en la productividad semanal de los Project Managers.
#### 1.2.2.2. Lean UX Assumptions
**Business Assumptions (Creencias del Negocio)**
1. Creemos que las organizaciones necesitan centralizar la visibilidad de sus proyectos y estandarizar la toma de decisiones basada en datos reales.
2. Creemos que estas necesidades se resuelven con una plataforma SaaS que integre gestion, monitoreo y control en una unica interfaz.
3. Creemos que nuestros primeros clientes seran empresas medianas y grandes con departamentos de PMO que sufren de desorden informativo.
4. Creemos que el modelo de ingresos sera una suscripcion B2B escalonada segun el volumen de proyectos o el numero de usuarios.
5. Creemos que nuestra ventaja competitiva sera la estandarizacion de procesos bajo metodologia PMO sin la friccion de herramientas genericas.

**Business Outcome Assumptions (Resultados del Negocio)**
1. Creemos que lograremos una reduccion del 25% en el tiempo de entrega de reportes operativos en los primeros 3 meses.
2. Creemos que obtendremos un incremento del 20% en la productividad semanal de los Project Managers al automatizar tareas de control.
3. Creemos que alcanzaremos 50 proyectos activos gestionados en la plataforma durante el primer ano.
4. Creemos que mantendremos una retencion de clientes superior al 90% tras los primeros 6 meses de uso.

**User Assumptions (Creencias sobre el Usuario)**
1. Creemos que nuestros usuarios principales son los Project Managers que ejecutan los proyectos y los Stakeholders que toman decisiones.
2. Creemos que la plataforma se utilizara en el seguimiento diario de hitos y en las reuniones semanales o mensuales de revision de desempeno.
3. Creemos que los usuarios buscan resolver la dispersion de la informacion que genera falta de control y decisiones tardias.

**User Outcome and Benefit Assumptions (Resultados y Beneficios para el Usuario)**
1. Creemos que los usuarios lograran visibilidad inmediata del estado de salud de todos los proyectos a traves de indicadores claros y semaforos de estado.
2. Creemos que los usuarios eliminaran la carga de trabajo estresante asociada a la recopilacion manual de datos para reportes.
3. Creemos que los usuarios lograran una asignacion optima de recursos humanos y financieros, reduciendo la desalineacion operativa.

**Feature Assumptions (Creencias sobre las Caracteristicas)**
1. Creemos que un **Dashboard Centralizado** reducira la desinformacion en las reuniones de seguimiento.
2. Creemos que un **Generador de Reportes Automatico** eliminara el 30% de la carga administrativa mensual.
3. Creemos que un **Sistema de Alertas Tempranas** notificara desviaciones para evitar el incumplimiento de plazos.
4. Creemos que un **Modulo de Gestion de Recursos** permitira la asignacion inteligente de personal y el seguimiento de tareas criticas.

#### 1.2.2.3. Lean UX Hypothesis Statements
##### Visualización y Control Centralizado
**Creemos que** al ofrecer un Dashboard en tiempo real con métricas unificadas, reduciremos los retrasos en la toma de decisiones estratégicas en un 20%. **Sabremos que estamos bien cuando veamos los siguientes comentarios del mercado:** "Ahora puedo ver el estado de todos mis proyectos en una sola pantalla" y/o los logs de la plataforma muestren que los Stakeholders consultan los dashboards diariamente antes de sus reuniones.

##### Automatización de Reporteo
**Creemos que** un generador automático de reportes de desempeño permitirá que los Project Managers recuperen un 30% de su productividad semanal. **Sabremos que estamos bien cuando veamos los siguientes comentarios del mercado:** "Generar el reporte mensual ahora me toma 5 minutos en lugar de dos días" y/o veamos una tasa de descarga de reportes superior al 80% al final de cada mes.

##### Estandarización de Procesos
**Creemos que** el uso de plantillas estandarizadas de gestión reducirá los errores de comunicación entre las áreas operativas y la PMO en un 25%. **Sabremos que estamos bien cuando veamos los siguientes comentarios del mercado:** "Todos los equipos hablamos el mismo lenguaje ahora" y/o se observe una reducción significativa en la cantidad de correos electrónicos aclaratorios sobre el estado de los proyectos.

##### Optimización de Recursos
**Creemos que** centralizar la asignación de recursos y seguimiento de hitos disminuirá los sobrecostos operativos por mala planificación. **Sabremos que estamos bien cuando veamos los siguientes comentarios del mercado:** "Tenemos menos cuellos de botella por falta de personal" y/o los indicadores financieros de los clientes muestren una mejora en el margen operativo de sus proyectos.

#### 1.2.2.4. Lean UX Canvas

| **Business Problem** | **Solutions** | **Business Outcomes** |
| :--- | :--- | :--- |
| El estado actual de la gestion de proyectos en organizaciones peruanas se caracteriza por una alta dependencia de procesos manuales, hojas de calculo aisladas y comunicacion fragmentada, lo que resulta en una perdida de productividad de hasta el 30%, sobrecostos operativos y falta de alineacion estrategica. Los productos existentes a menudo son demasiado complejos o costosos para las PMO que buscan una estandarizacion rapida sin una curva de aprendizaje tecnica elevada. **MDEPS** busca cerrar esta brecha mediante una plataforma web centralizada que automatice el control de hitos, proporcione visibilidad en tiempo real y unifique los datos para la toma de decisiones. Nuestro enfoque inicial sera satisfacer las necesidades de los Project Managers y Stakeholders de empresas medianas y grandes. Sabremos que hemos tenido exito cuando reduzcamos los tiempos de reporteo, disminuyamos los retrasos en hitos y aumentemos la confiabilidad de la informacion para la gerencia. | **- Dashboard de control centralizado:** Visualizacion 360 grados de la salud de todos los portafolios de proyectos en tiempo real.<br><br>**- Generacion automatica de reportes:** Modulo que consolida KPIs de desempeno y los exporta de forma instantanea, eliminando la carga manual.<br><br>**- Sistema de alertas tempranas:** Notificaciones automaticas ante desviaciones de cronograma (hitos) o presupuesto.<br><br>**- Modulo de gestion de recursos:** Herramientas para la asignacion inteligente de personal y seguimiento de tareas criticas. | - Reduccion del 25% en el tiempo dedicado a la elaboracion de reportes mensuales.<br><br>- Disminucion del 15% en los sobrecostos por retrasos no detectados a tiempo.<br><br>- Incremento del 20% en la productividad semanal de los Project Managers.<br><br>- Alcanzar 50 proyectos activos gestionados integramente en la plataforma en el primer ano.<br><br>- Retencion de clientes B2B superior al 90% tras el primer semestre de implementacion. |

| **Users** | **User Outcomes & Benefits** |
| :--- | :--- |
| **- Project Managers:** "Nuestro objetivo es dejar de perder tiempo en Excel y asegurar que el equipo cumpla con los plazos establecidos."<br><br>**- PMO Leads / Jefes de Proyecto:** "Nuestro objetivo es estandarizar la metodologia de trabajo en toda la empresa para que la informacion sea comparable y confiable."<br><br>**- Stakeholders / Ejecutivos:** "Nuestro objetivo es tener visibilidad clara del ROI y el avance de los proyectos estrategicos para tomar decisiones informadas sin esperar a la reunion mensual." | **- Project Managers:** Optimizacion de su tiempo operativo, eliminacion de tareas administrativas repetitivas y mayor control sobre sus equipos. **Beneficios:** Menos estres por reporteo, alertas proactivas y mayor cumplimiento de cronogramas. **Indicadores:** Horas ahorradas por semana y reduccion de correos de seguimiento.<br><br>**- PMO Leads:** Informacion estandarizada y centralizada de todos los portafolios, facilitando la auditoria y mejora de procesos. **Beneficios:** Trazabilidad total de la operacion y reduccion de silos de informacion. **Indicadores:** Mayor precision en las proyecciones de cierre de proyecto.<br><br>**- Stakeholders:** Acceso a dashboards ejecutivos que permiten ver el "semaforo" de la empresa en segundos. **Beneficios:** Tranquilidad estrategica y capacidad de intervencion temprana en proyectos criticos. **Indicadores:** Mejora en el margen operativo y alineacion de resultados con objetivos anuales. |

| **Hypotheses** | **What's the most important thing we need to learn first?** | **What's the least amount of work we need to do to learn the next most important thing?** |
| :--- | :--- | :--- |
| **- Creemos que** reduciremos el tiempo de reporteo en un 25% si los Project Managers utilizan el generador automatico de reportes de **MDEPS** en lugar de consolidar datos manualmente en Excel.<br><br>**- Creemos que** disminuiremos los sobrecostos operativos en un 15% si los PMO Leads reciben alertas tempranas de desviaciones presupuestarias a traves de nuestro sistema de monitoreo en tiempo real.<br><br>**- Creemos que** aumentaremos la satisfaccion de los Stakeholders en un 40% si obtienen acceso directo a tableros de control ejecutivos que muestren el avance estrategico del portafolio.<br><br>**- Creemos que** alcanzaremos una adopcion de 50 proyectos activos en un ano si ofrecemos una interfaz intuitiva con onboarding guiado que no requiera capacitacion tecnica externa.<br><br>**- Creemos que** mejoraremos la eficiencia del equipo en un 20% si los recursos se asignan de manera centralizada evitando la sobrecarga de trabajo y los cuellos de botella. | - ¿Es la recopilacion manual de datos el problema mas doloroso para los Project Managers, o existe otra friccion mayor en su dia a dia?<br><br>- ¿Estan los ejecutivos dispuestos a basar sus decisiones financieras en un dashboard digital en lugar de esperar los reportes tradicionales firmados?<br><br>- ¿La estandarizacion de procesos es percibida como una ayuda o como una restriccion burocratica por los equipos de ingenieria?<br><br>- ¿Es la integracion con herramientas actuales (como Excel) una funcionalidad critica para que acepten migrar a nuestra plataforma?<br><br>- ¿Cual es el KPI especifico que mas valoran los Stakeholders para considerar que un proyecto esta "bajo control"? | - Realizar entrevistas a profundidad con 5 lideres de PMO y Project Managers para validar sus "pain points" prioritarios.<br><br>- Crear un prototipo navegable de alta fidelidad (Figma) que simule el dashboard y el generador de reportes para realizar pruebas de concepto con usuarios reales.<br><br>- Realizar una prueba piloto con una oficina de proyectos pequena (3-5 proyectos) cargando datos historicos para comparar la precision de **MDEPS** vs su gestion manual previa.<br><br>- Encuesta a Stakeholders para priorizar los 3 KPIs mas importantes que necesitan ver en un panel ejecutivo. |

---

## 1.3. Segmentos objetivo
### Segmento 1: Líderes y Jefes de Gestión de Proyectos

Corresponde a los usuarios directos y principales adoptantes de la plataforma. Esta conformado por profesionales de entre 30 y 50 anos, con formacion solida en Ingenieria o Administracion y, frecuentemente, con certificaciones internacionales como el PMP o especializaciones en metodologias agiles. Su dia a dia se ve afectado por la frustracion de realizar un seguimiento reactivo basado en datos fragmentados y canales informales como WhatsApp o correos electronicos. Psicograficamente, estos lideres valoran la precision informativa y buscan herramientas que les permitan predecir desviaciones de presupuesto o cronograma antes de que ocurran. Estadisticamente, se estima que un jefe de proyectos en el Peru invierte hasta un 30% de su jornada semanal unicamente en la consolidacion manual de informes, una carga administrativa que se busca erradicar para permitirles enfocarse en la estrategia y la eficiencia del equipo.

### Segmento 2: Empresas Medianas y Grandes con Múltiples Portafolios

Define a nivel corporativo el mercado B2B donde la solucion genera un impacto economico directo. Estas organizaciones, pertenecientes a sectores de alta complejidad como Construccion, Mineria, Consultoria de TI e Ingenieria, gestionan simultaneamente entre 5 y 20 proyectos con recursos y presupuestos compartidos. Son empresas que han superado su capacidad de control mediante herramientas basicas como hojas de calculo y sufren de una "ceguera operativa" que impide a la alta gerencia conocer el estado real de sus inversiones en tiempo real. En el mercado local, esta falta de visibilidad se traduce en sobrecostos que oscilan entre el 10% y el 15% del presupuesto total de cada proyecto. Para estas organizaciones, la adopcion de una solucion centralizada no es solo una mejora tecnologica, sino una necesidad critica para mantener la rentabilidad, asegurar la gobernanza de datos y evitar penalidades por incumplimiento de plazos contractuales.