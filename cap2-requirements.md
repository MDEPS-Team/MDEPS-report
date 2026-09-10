# Capitulo II: Requirements Development and Software Solution Design
La recolección y análisis de requisitos es una etapa fundamental en el desarrollo de Vantage PMO, ya que permite identificar y comprender las necesidades de los stakeholders involucrados en la gestión de proyectos. Para ello, se emplean técnicas como el análisis de la competencia y las entrevistas a usuarios pertenecientes a los segmentos objetivo.

A través de este análisis se busca identificar problemáticas relacionadas con la falta de visibilidad, la fragmentación de la información, las dificultades en el seguimiento de proyectos y la ausencia de estandarización en los procesos. Los resultados obtenidos permitirán definir las necesidades y requerimientos más relevantes de los usuarios, estableciendo una base para el diseño de una solución que facilite la gestión de proyectos y contribuya a una toma de decisiones más oportuna.
## 2.1. Competidores
En esta sección se analizan las principales soluciones existentes en el mercado relacionadas con la gestión de proyectos y portafolios. El objetivo es identificar sus principales características, ventajas y limitaciones para determinar oportunidades de diferenciación para Vantage PMO.

Los competidores seleccionados son Jira, monday.com y Planview Portfolios, debido a que ofrecen funcionalidades relacionadas con la planificación, seguimiento, visualización, gestión de recursos y toma de decisiones en proyectos.

Jira

Jira es una plataforma de gestión del trabajo ampliamente utilizada, especialmente en equipos de desarrollo de software. Permite planificar y asignar actividades, realizar seguimiento mediante tableros y cronogramas, automatizar flujos de trabajo y generar reportes y dashboards. También permite visualizar métricas y el estado de los proyectos para facilitar la toma de decisiones.

Su principal ventaja es su alto nivel de personalización y la gran cantidad de funcionalidades e integraciones disponibles. Sin embargo, su enfoque está fuertemente relacionado con la gestión del trabajo y el desarrollo de software, por lo que Vantage PMO puede diferenciarse mediante una experiencia más enfocada en la supervisión integral de portafolios y procesos de PMO.

monday.com

monday.com es una plataforma visual de gestión de proyectos y trabajo que permite organizar actividades, responsables, cronogramas y recursos. Cuenta con diagramas de Gantt, dashboards, gestión de carga de trabajo, hitos y automatizaciones. Sus dashboards permiten centralizar información de diferentes proyectos para facilitar el seguimiento y la toma de decisiones.

Su principal fortaleza es la facilidad de personalización y la experiencia visual. Sin embargo, al ser una plataforma generalista, Vantage PMO puede diferenciarse mediante funcionalidades diseñadas específicamente para las necesidades de una PMO, como estandarización de procesos, seguimiento de portafolios y generación de información ejecutiva.

Planview Portfolios

Planview Portfolios es una solución orientada directamente a la gestión de portafolios de proyectos. Permite conectar la estrategia empresarial con proyectos, gestionar recursos y capacidad, priorizar iniciativas, controlar aspectos financieros y generar dashboards y reportes para la toma de decisiones.

Su principal ventaja es su orientación hacia la gestión estratégica de portafolios y organizaciones de gran escala. Como oportunidad para Vantage PMO, se puede plantear una experiencia más sencilla y accesible para organizaciones que necesitan centralizar el seguimiento de proyectos sin enfrentarse a la complejidad de una plataforma empresarial de gran escala.

### 2.1.1 Análisis competitivo
<a id="2-1-1-analisis-competitivo"></a>

| **¿Por qué llevar a cabo este análisis?** | Evaluar el posicionamiento de Vantage PMO frente a sus competidores para identificar oportunidades de diferenciación y definir estrategias competitivas. |
| ----------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- |

| **Categoría** | **Vantage PMO (Startup)** | **Jira** | **Monday.com** | **Planview Portfolios** |
| ------------------------------------------ | ---------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------- | ---------------------------------------------------------------- | ---------------------------------------------------------------- |
| **Perfil** | | | | |
| **Overview** | Plataforma orientada a centralizar la gestión y supervisión de proyectos y portafolios, proporcionando dashboards, reportes y control de recursos. | Plataforma de gestión del trabajo y proyectos, especialmente utilizada en equipos de desarrollo de software. | Plataforma visual y personalizable para gestionar proyectos, tareas, recursos y flujos de trabajo. | Plataforma empresarial especializada en la gestión estratégica de portafolios y proyectos. |
| **Ventaja competitiva (valor al cliente)** | Centralización de información, visibilidad de proyectos y enfoque específico en las necesidades de una PMO. | Alta personalización, automatización e integración con herramientas de desarrollo. | Facilidad de uso, flexibilidad y visualización de información. | Gestión integral de portafolios, recursos, planificación, análisis y alineación estratégica. |
| **Perfil de Marketing** | | | | |
| **Mercado objetivo** | Empresas medianas y grandes que gestionan múltiples proyectos y requieren mayor visibilidad y estandarización. | Equipos de desarrollo de software y organizaciones que gestionan diferentes tipos de trabajo. | Equipos y empresas que buscan organizar proyectos y procesos de manera flexible. | Empresas y organizaciones de gran escala con necesidades de gestión de portafolios y recursos. |
| **Estrategias de marketing** | Enfoque en productividad, centralización de información y transformación digital de la gestión de proyectos. | Posicionamiento dentro del ecosistema tecnológico, integraciones y gestión del trabajo de desarrollo. | Comunicación centrada en facilidad de uso, personalización, colaboración y gestión visual. | Posicionamiento empresarial basado en gestión estratégica, optimización de recursos y toma de decisiones basada en datos. |
| **Perfil de Producto** | | | | |
| **Productos & Servicios** | Dashboards, seguimiento de proyectos, reportes, gestión de recursos y centralización de información. | Gestión de tareas, tableros, cronogramas, automatizaciones, reportes y dashboards. | Gestión de proyectos, tableros, Gantt, dashboards, automatizaciones y gestión de carga de trabajo. | Gestión de portafolios, planificación, recursos, proyectos, riesgos, reportes, dashboards y análisis. |
| **Precios & Costos** | Modelo SaaS por definir de acuerdo con el alcance de la solución. | Cuenta con opciones gratuitas y planes de pago según funcionalidades y necesidades. | Modelo de suscripción con diferentes planes según las necesidades de los equipos y organizaciones. | Orientado principalmente al mercado empresarial; precios bajo cotización. |
| **Canales de distribución** | Web / Móvil | Web / Móvil | Web / Móvil | Web / Plataformas empresariales |
| **Análisis SWOT** | | | | |
| **Fortalezas** | • Centralización de información. <br> • Enfoque específico en PMO. <br> • Interfaz orientada a facilitar la visualización de proyectos. | • Alta personalización. <br> • Amplio ecosistema de integraciones. <br> • Amplio reconocimiento en equipos tecnológicos. | • Interfaz visual. <br> • Flexible y personalizable. <br> • Facilidad para organizar diferentes tipos de trabajo. | • Especialización en gestión de portafolios. <br> • Gestión de recursos y capacidad. <br> • Dashboards y análisis avanzados. |
| **Debilidades** | • Producto nuevo. <br> • Menor reconocimiento de marca. <br> • Menor cantidad de integraciones en comparación con plataformas consolidadas. | • Puede resultar complejo para usuarios no familiarizados con herramientas de gestión de desarrollo. <br> • Requiere configuración para adaptarse a diferentes necesidades. | • Menor especialización en gestión estratégica de PMO frente a plataformas PPM especializadas. | • Mayor complejidad. <br> • Orientación principalmente empresarial. <br> • Puede resultar menos accesible para organizaciones pequeñas o con necesidades más simples. |
| **Oportunidades** | • Crecimiento de la digitalización empresarial. <br> • Empresas que aún dependen de herramientas dispersas. <br> • Mayor necesidad de visibilidad sobre múltiples proyectos. | • Expansión hacia diferentes áreas de gestión del trabajo. <br> • Nuevas integraciones y automatizaciones. | • Crecimiento del trabajo colaborativo y digital. <br> • Adopción en diferentes sectores empresariales. | • Creciente demanda de soluciones de Project Portfolio Management. <br> • Incorporación de inteligencia artificial y análisis avanzado. |
| **Amenazas** | • Competidores consolidados. <br> • Nuevas startups de gestión de proyectos. <br> • Evolución rápida de las tecnologías de gestión. | • Competencia de plataformas de gestión de proyectos y trabajo colaborativo. <br> • Cambios rápidos en las necesidades de los equipos. | • Competidores especializados en diferentes industrias. <br> • Saturación del mercado de gestión de proyectos. | • Competencia de soluciones PPM y SPM. <br> • Evolución de plataformas más simples y accesibles. |

### 2.1.2. Estrategias y tacticas frente a competidores
Para diferenciar Vantage PMO frente a las soluciones existentes, se plantean las siguientes estrategias y tácticas:

1. Especialización en gestión de PMO

Estrategia:
Diferenciar Vantage PMO mediante funcionalidades orientadas específicamente a la gestión y supervisión de portafolios de proyectos.

Táctica:
Desarrollar dashboards ejecutivos, seguimiento de hitos, indicadores y herramientas de control que permitan visualizar el estado de múltiples proyectos desde una misma plataforma.

2. Simplificación de la experiencia de usuario

Estrategia:
Ofrecer una experiencia sencilla que reduzca la complejidad de las herramientas empresariales de gestión de proyectos.

Táctica:
Diseñar una interfaz intuitiva, con navegación clara, información priorizada y dashboards visuales que permitan consultar rápidamente el estado de los proyectos.

3. Centralización de la información

Estrategia:
Reducir la dispersión de información entre diferentes herramientas y canales de comunicación.

Táctica:
Centralizar información relacionada con proyectos, responsables, recursos, avances, hitos y reportes dentro de una misma plataforma.

4. Soporte para la toma de decisiones

Estrategia:
Convertir la información de los proyectos en indicadores útiles para los responsables de la organización.

Táctica:
Implementar dashboards, indicadores clave de desempeño (KPIs), alertas y reportes que permitan detectar desviaciones y tomar decisiones oportunamente.

5. Automatización de procesos

Estrategia:
Reducir el tiempo dedicado a actividades administrativas y recopilación manual de información.

Táctica:
Automatizar la generación de reportes, actualización de información y alertas relacionadas con hitos, fechas límite y posibles desviaciones.

6. Compatibilidad con herramientas existentes

Estrategia:
Disminuir la resistencia al cambio y facilitar la incorporación de Vantage PMO en organizaciones que ya utilizan otras herramientas.

Táctica:
Considerar mecanismos de importación y exportación de información y futuras integraciones con herramientas utilizadas habitualmente por los equipos de proyectos.

---

## 2.2. Entrevistas

### 2.2.1. Diseno de entrevistas
Las entrevistas tienen como objetivo conocer las experiencias, necesidades, dificultades y expectativas de los usuarios relacionados con la gestión de múltiples proyectos. Las preguntas fueron diseñadas para obtener información sobre sus actividades actuales, herramientas utilizadas, problemas frecuentes, toma de decisiones y disposición para utilizar una solución centralizada como Vantage PMO.

#### Preguntas de presentación

- ¿Cuál es su nombre?
- ¿Cuántos años tiene?
- ¿En qué distrito reside?
- ¿Cuál es su ocupación o cargo actual?
- ¿Cuántos años de experiencia tiene en su área?

### Segmento 1: Líderes o jefes de gestión de proyectos

#### Preguntas principales

1. ¿Cuál es tu rol dentro de la organización y cuáles son tus principales responsabilidades en la gestión de proyectos?

2. ¿Cuántos proyectos sueles gestionar o supervisar de manera simultánea?

3. ¿Qué herramientas utilizas actualmente para organizar y hacer seguimiento de tus proyectos?

4. ¿Cómo realizas actualmente el seguimiento del avance de los proyectos y con qué frecuencia lo haces?

5. ¿Qué información consideras indispensable para conocer rápidamente el estado de un proyecto?

6. ¿Cuál es la principal dificultad que encuentras al gestionar varios proyectos al mismo tiempo?

7. ¿Has tenido problemas debido a que la información de los proyectos se encuentra dispersa, desactualizada o en diferentes herramientas? ¿Podrías contarnos algún ejemplo?

8. ¿Qué actividades relacionadas con el seguimiento o elaboración de reportes consideras que te quitan más tiempo?

9. Si tuvieras una plataforma centralizada para gestionar tus proyectos, ¿qué funcionalidades considerarías más útiles?

10. ¿Estarías dispuesto(a) a utilizar una plataforma de este tipo? ¿Qué características tendría que tener para que realmente te resulte útil?
#### Preguntas complementarias

- ¿Con qué frecuencia revisa el estado de sus proyectos?
- ¿Qué dispositivo utiliza con mayor frecuencia para consultar información de sus proyectos?
- ¿Qué información le gustaría poder consultar rápidamente desde un dispositivo móvil?
- ¿Qué cambiaría de las herramientas que utiliza actualmente?
- ¿Ha tenido que utilizar hojas de cálculo, correo electrónico o aplicaciones de mensajería para complementar sus herramientas de gestión? ¿Por qué?

### Segmento 2: Empresas medianas y grandes con múltiples proyectos

#### Preguntas principales

1. ¿A qué se dedica la organización y cuál es tu función dentro de ella?

2. ¿Cuántos proyectos o iniciativas suelen manejar simultáneamente?

3. ¿Cómo organizan actualmente la información sobre proyectos, tareas, responsables y fechas?

4. ¿Qué herramientas utilizan actualmente para gestionar o hacer seguimiento de sus proyectos?

5. ¿Cómo se comparte la información sobre el avance de los proyectos entre las diferentes personas o áreas?

6. ¿Cuál es la principal dificultad que tienen actualmente para coordinar varios proyectos?

7. ¿Han tenido problemas con retrasos, falta de coordinación o pérdida de información? ¿Podrías contarnos algún ejemplo?

8. ¿Qué información necesitarías consultar rápidamente para conocer el estado de todos los proyectos?

9. ¿Qué funcionalidades considerarías importantes en una plataforma centralizada para gestionar los proyectos de la organización?

10. ¿Qué condiciones tendría que cumplir una nueva plataforma para que la organización estuviera dispuesta a adoptarla?
#### Preguntas complementarias

- ¿Qué herramienta utilizan con mayor frecuencia durante su jornada laboral?
- ¿Utilizan principalmente computadora, tablet o teléfono móvil para realizar estas actividades?
- ¿Qué información les gustaría consultar desde un dispositivo móvil?
- ¿Qué problema de la gestión actual les gustaría solucionar primero?
- ¿Qué factores podrían dificultar la adopción de una nueva herramienta dentro de la empresa?
### 2.2.2. Registro de entrevistas

En esta sección presentamos los registros de las entrevistas realizadas a personas pertenecientes a los segmentos objetivo de Vantage PMO. El objetivo de las entrevistas fue conocer sus experiencias, dificultades y necesidades relacionadas con la gestión y seguimiento de múltiples proyectos, así como identificar oportunidades de mejora mediante una plataforma centralizada.

### Segmento 1: Líderes y Jefes de Gestión de Proyectos

<table>
<thead>
  <tr>
    <th colspan="2">Entrevista #1</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Nombre</td>
    <td>Gerson</td>
  </tr>
  <tr>
    <td>Apellidos</td>
    <td>Escarate</td>
  </tr>
  <tr>
    <td>Edad</td>
    <td>30 años</td>
  </tr>
  <tr>
    <td>Distrito</td>
    <td>Surco</td>
  </tr>
  <tr>
    <td>Ocupación</td>
    <td>Project Manager</td>
  </tr>
  <tr>
    <td>Evidencia</td>
    <td>Por agregar</td>
  </tr>
  <tr>
    <td>Link</td>
    <td>Por agregar</td>
  </tr>
  <tr>
    <td>Duración</td>
    <td>Por agregar</td>
  </tr>
  <tr>
    <td>Resumen</td>
    <td>
      Gerson se desempeña como Project Manager en el sector tecnológico y cuenta con aproximadamente cinco años de experiencia en gestión de proyectos. Actualmente supervisa alrededor de seis proyectos de manera simultánea y utiliza herramientas como Jira, Microsoft Project y Excel para organizar y realizar el seguimiento de las actividades. Realiza un seguimiento frecuente del avance de los proyectos y considera importante contar con información actualizada sobre el progreso, responsables, fechas y recursos disponibles. Entre las principales dificultades que identifica se encuentra la consolidación de información proveniente de diferentes herramientas, especialmente al momento de preparar reportes. Considera que una plataforma centralizada con dashboards, alertas y seguimiento de indicadores podría reducir el trabajo administrativo y facilitar la toma de decisiones. También considera importante que la herramienta sea sencilla de utilizar y que pueda accederse desde dispositivos móviles.
    </td>
  </tr>
</tbody>
</table>


<table>
<thead>
  <tr>
    <th colspan="2">Entrevista #2</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Nombre</td>
    <td>Lucy</td>
  </tr>
  <tr>
    <td>Apellidos</td>
    <td>Linares</td>
  </tr>
  <tr>
    <td>Edad</td>
    <td>28 años</td>
  </tr>
  <tr>
    <td>Distrito</td>
    <td>Miraflores</td>
  </tr>
  <tr>
    <td>Ocupación</td>
    <td>Coordinadora de proyectos</td>
  </tr>
  <tr>
    <td>Evidencia</td>
    <td>Por agregar</td>
  </tr>
  <tr>
    <td>Link</td>
    <td>Por agregar</td>
  </tr>
  <tr>
    <td>Duración</td>
    <td>Por agregar</td>
  </tr>
  <tr>
    <td>Resumen</td>
    <td>
      Lucy trabaja como coordinadora de proyectos y participa en la supervisión de entre cuatro y siete proyectos simultáneamente. Para organizar la información utiliza principalmente Excel, documentos compartidos y Microsoft Teams. Realiza reuniones periódicas para conocer el avance de las actividades, aunque señala que uno de los problemas es mantener actualizada la información cuando participan diferentes responsables. También identifica la elaboración y actualización de reportes como una actividad que consume tiempo. Considera que una herramienta centralizada con dashboards y alertas permitiría visualizar rápidamente el estado de los proyectos y detectar posibles retrasos. Para adoptar una nueva solución considera importante que sea intuitiva y que no requiera un proceso de aprendizaje complejo.
    </td>
  </tr>
</tbody>
</table>


<table>
<thead>
  <tr>
    <th colspan="2">Entrevista #3</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Nombre</td>
    <td>Christopher</td>
  </tr>
  <tr>
    <td>Apellidos</td>
    <td>Osorio</td>
  </tr>
  <tr>
    <td>Edad</td>
    <td>38 años</td>
  </tr>
  <tr>
    <td>Distrito</td>
    <td>San Borja</td>
  </tr>
  <tr>
    <td>Ocupación</td>
    <td>Jefe de proyectos</td>
  </tr>
  <tr>
    <td>Evidencia</td>
    <td>Por agregar</td>
  </tr>
  <tr>
    <td>Link</td>
    <td>Por agregar</td>
  </tr>
  <tr>
    <td>Duración</td>
    <td>Por agregar</td>
  </tr>
  <tr>
    <td>Resumen</td>
    <td>
      Christopher se desempeña como jefe de proyectos y tiene bajo su responsabilidad aproximadamente ocho proyectos de manera simultánea. Para realizar el seguimiento utiliza Microsoft Project, Excel y sistemas internos de la organización. Considera necesario disponer de una visión general que le permita identificar rápidamente el avance de cada proyecto, sus fechas importantes y posibles desviaciones. Una de las actividades que considera más demandantes es la preparación y consolidación de información para reportes. Entre las funcionalidades que considera útiles en una plataforma centralizada menciona dashboards, filtros, indicadores y alertas. También considera que la facilidad de uso es un factor importante para que los integrantes del equipo puedan adoptar una nueva herramienta.
    </td>
  </tr>
</tbody>
</table>


### Segmento 2: Empresas medianas y grandes con múltiples proyectos

<table>
<thead>
  <tr>
    <th colspan="2">Entrevista #1</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Nombre</td>
    <td>Katherine</td>
  </tr>
  <tr>
    <td>Apellidos</td>
    <td>Herrera Cotrina</td>
  </tr>
  <tr>
    <td>Edad</td>
    <td>37 años</td>
  </tr>
  <tr>
    <td>Distrito</td>
    <td>Ancón</td>
  </tr>
  <tr>
    <td>Ocupación</td>
    <td>Coordinadora de operaciones</td>
  </tr>
  <tr>
    <td>Evidencia</td>
    <td>Por agregar</td>
  </tr>
  <tr>
    <td>Link</td>
    <td>Por agregar</td>
  </tr>
  <tr>
    <td>Duración</td>
    <td>Por agregar</td>
  </tr>
  <tr>
    <td>Resumen</td>
    <td>
      Katherine se desempeña como coordinadora de operaciones en una organización donde participa en la gestión de diferentes proyectos e iniciativas. Para organizar las actividades utiliza principalmente Excel, Google Drive y WhatsApp, y ocasionalmente otras herramientas de gestión. Identifica como una de sus principales dificultades la dispersión de información entre diferentes herramientas y canales de comunicación. El seguimiento de fechas, tareas y responsables puede complicarse cuando existen varios proyectos simultáneos. Considera que una plataforma centralizada con alertas y recordatorios facilitaría el control de las actividades y reduciría los problemas de coordinación. Para adoptar una nueva solución considera fundamental que sea fácil de utilizar y que requiera poca capacitación.
    </td>
  </tr>
</tbody>
</table>


<table>
<thead>
  <tr>
    <th colspan="2">Entrevista #2</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Nombre</td>
    <td>James</td>
  </tr>
  <tr>
    <td>Apellidos</td>
    <td>Jara</td>
  </tr>
  <tr>
    <td>Edad</td>
    <td>34 años</td>
  </tr>
  <tr>
    <td>Distrito</td>
    <td>San Miguel</td>
  </tr>
  <tr>
    <td>Ocupación</td>
    <td>Administrador de empresa</td>
  </tr>
  <tr>
    <td>Evidencia</td>
    <td>Por agregar</td>
  </tr>
  <tr>
    <td>Link</td>
    <td>Por agregar</td>
  </tr>
  <tr>
    <td>Duración</td>
    <td>Por agregar</td>
  </tr>
  <tr>
    <td>Resumen</td>
    <td>
      James trabaja en la administración de una empresa que desarrolla diferentes iniciativas de manera simultánea. Actualmente utiliza Excel, correo electrónico y documentos compartidos para organizar la información. Señala que uno de los principales inconvenientes es la existencia de diferentes versiones de los documentos y la posibilidad de trabajar con información desactualizada. Para realizar el seguimiento considera importante conocer las fechas, responsables y estado de las tareas. Considera que una plataforma centralizada permitiría mejorar la organización y reducir la duplicidad de información. Entre las funcionalidades que considera más útiles se encuentran los recordatorios y una vista general de los proyectos. Para adoptar una nueva herramienta considera importante que sea sencilla y práctica para los usuarios.
    </td>
  </tr>
</tbody>
</table>


<table>
<thead>
  <tr>
    <th colspan="2">Entrevista #3</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Nombre</td>
    <td>Alessandro</td>
  </tr>
  <tr>
    <td>Apellidos</td>
    <td>Nieto</td>
  </tr>
  <tr>
    <td>Edad</td>
    <td>29 años</td>
  </tr>
  <tr>
    <td>Distrito</td>
    <td>Los Olivos</td>
  </tr>
  <tr>
    <td>Ocupación</td>
    <td>Coordinador de proyectos</td>
  </tr>
  <tr>
    <td>Evidencia</td>
    <td>Por agregar</td>
  </tr>
  <tr>
    <td>Link</td>
    <td>Por agregar</td>
  </tr>
  <tr>
    <td>Duración</td>
    <td>Por agregar</td>
  </tr>
  <tr>
    <td>Resumen</td>
    <td>
      Alessandro participa en la coordinación de diferentes proyectos y actividades de manera simultánea. Para organizar su trabajo utiliza principalmente WhatsApp, Excel y Trello. Considera que uno de los principales problemas es la dificultad para obtener una visión general de todos los proyectos, especialmente cuando la información se encuentra distribuida en diferentes herramientas. Para realizar un seguimiento adecuado considera necesario conocer las fechas, responsables y tareas pendientes. También considera útiles las notificaciones y recordatorios para evitar que se pasen fechas importantes. Estaría dispuesto a utilizar una plataforma centralizada si esta permite ahorrar tiempo, mejorar la organización y resulta sencilla de utilizar.
    </td>
  </tr>
</tbody>
</table>

<a id="2-2-3-analisis-de-entrevistas"></a>

## 2.2.3 Análisis de Entrevistas

### Segmento 1: Líderes y Jefes de Gestión de Proyectos

Se analizaron 3 entrevistas a personas que desempeñan funciones relacionadas con la gestión y coordinación de proyectos. La información recopilada permitió identificar características objetivas y subjetivas comunes relacionadas con la cantidad de proyectos gestionados, las herramientas utilizadas, las dificultades de seguimiento y las necesidades de información para la toma de decisiones. Estos resultados servirán como base para la construcción de los User Personas y la identificación de oportunidades para Vantage PMO.

| Característica | Mención | % | Evidencia |
| :--- | :---: | :---: | :--- |
| **Gestión simultánea de múltiples proyectos** | 3/3 | 100% | Gerson, Lucy y Christopher mencionan que gestionan o supervisan varios proyectos de manera simultánea. |
| **Uso de herramientas digitales para la gestión** | 3/3 | 100% | Los tres entrevistados utilizan herramientas como Jira, Microsoft Project, Excel, documentos compartidos o sistemas internos. |
| **Seguimiento frecuente del avance de los proyectos** | 3/3 | 100% | Los entrevistados realizan un seguimiento frecuente para conocer el avance de las tareas y el estado de sus proyectos. |
| **Importancia de contar con información actualizada** | 3/3 | 100% | Los tres consideran importante conocer información sobre avances, responsables, fechas y recursos para controlar los proyectos. |
| **Dificultades para consolidar información** | 3/3 | 100% | Los entrevistados mencionan dificultades relacionadas con la información distribuida entre diferentes herramientas o responsables. |
| **Elaboración de reportes como actividad que consume tiempo** | 2/3 | 66,6% | Gerson y Lucy identifican la elaboración o actualización de reportes como una actividad que demanda tiempo. |
| **Necesidad de visualizar retrasos o desviaciones** | 3/3 | 100% | Los entrevistados consideran importante identificar oportunamente retrasos, avances y posibles desviaciones. |
| **Interés en dashboards o información centralizada** | 3/3 | 100% | Gerson, Lucy y Christopher consideran útil contar con una vista centralizada del estado de los proyectos. |
| **Importancia de alertas y recordatorios** | 2/3 | 66,6% | Gerson y Christopher mencionan las alertas o recordatorios como funcionalidades útiles para realizar seguimiento. |
| **Importancia de la facilidad de uso** | 3/3 | 100% | Los tres entrevistados consideran importante que una nueva plataforma sea intuitiva y sencilla de utilizar. |

### Insights Destacados

* **La gestión simultánea de proyectos requiere un seguimiento constante:** El 100% de los entrevistados gestiona o supervisa múltiples proyectos, por lo que necesitan consultar frecuentemente el avance, las fechas y las responsabilidades asociadas a cada proyecto.

* **La información dispersa dificulta el control de los proyectos:** El 100% de los entrevistados utiliza diferentes herramientas para organizar la información. Esta distribución puede dificultar la consolidación y consulta de los datos necesarios para conocer el estado general de los proyectos.

* **La visibilidad del estado de los proyectos es una necesidad común:** El 100% considera importante disponer de información actualizada sobre avances, responsables y fechas. Esto evidencia una oportunidad para Vantage PMO mediante dashboards que permitan consultar la información de manera centralizada.

* **Los reportes representan una oportunidad de optimización:** El 66,6% de los entrevistados identifica la elaboración o actualización de reportes como una actividad que consume tiempo. Esto respalda la incorporación de funcionalidades que faciliten la generación y consulta de reportes.

* **La facilidad de uso es fundamental para la adopción:** El 100% de los entrevistados considera importante que una nueva herramienta sea sencilla e intuitiva. Por ello, Vantage PMO debe priorizar una experiencia de usuario clara y evitar una curva de aprendizaje innecesariamente elevada.

---

### Segmento 2: Empresas Medianas y Grandes con Múltiples Proyectos

Se analizaron 3 entrevistas a personas que participan en organizaciones o actividades donde se gestionan múltiples proyectos de manera simultánea. La información recopilada permitió identificar problemas relacionados con la organización de tareas, la dispersión de información, la coordinación entre responsables y la necesidad de contar con una herramienta que facilite el control de los proyectos.

| Característica | Mención | % | Evidencia |
| :--- | :---: | :---: | :--- |
| **Gestión simultánea de múltiples proyectos o iniciativas** | 3/3 | 100% | Katherine, James y Alessandro mencionan que participan en la gestión de múltiples proyectos o actividades de manera simultánea. |
| **Uso de herramientas no centralizadas** | 3/3 | 100% | Los tres utilizan diferentes herramientas como Excel, Google Drive, WhatsApp, correo electrónico o Trello. |
| **Información dispersa entre diferentes herramientas** | 3/3 | 100% | Los entrevistados identifican dificultades relacionadas con tener información distribuida entre diferentes herramientas y canales de comunicación. |
| **Dificultades para realizar seguimiento de tareas y fechas** | 3/3 | 100% | Katherine, James y Alessandro consideran necesario realizar un seguimiento de tareas, responsables y fechas para mantener el control. |
| **Dependencia de herramientas de comunicación informal** | 2/3 | 66,6% | Katherine y Alessandro utilizan principalmente WhatsApp como parte de la coordinación de sus actividades. |
| **Necesidad de centralizar la información** | 3/3 | 100% | Los tres entrevistados consideran útil contar con una plataforma que reúna la información de los proyectos en un solo lugar. |
| **Importancia de alertas y recordatorios** | 2/3 | 66,6% | Katherine y Alessandro consideran útiles las alertas o recordatorios para evitar olvidos y controlar fechas importantes. |
| **Importancia de la facilidad de uso** | 3/3 | 100% | Los tres entrevistados consideran que una nueva herramienta debe ser sencilla y práctica para facilitar su adopción. |
| **Interés en acceder a la información desde dispositivos móviles** | 1/3 | 33,3% | Alessandro menciona el acceso móvil como una característica útil para consultar y gestionar información. |
| **Problemas relacionados con información duplicada o desactualizada** | 2/3 | 66,6% | Katherine y James mencionan dificultades relacionadas con la duplicidad o actualización de información cuando se utilizan diferentes herramientas. |

### Insights Destacados

* **La gestión de múltiples proyectos se apoya principalmente en herramientas independientes:** El 100% de los entrevistados utiliza diferentes herramientas para organizar y coordinar sus actividades. Esto evidencia la necesidad de contar con una solución que permita centralizar la información relacionada con proyectos, tareas, responsables y fechas.

* **La falta de centralización dificulta el seguimiento:** El 100% de los entrevistados identifica problemas relacionados con la distribución de información. Cuando los datos se encuentran en diferentes herramientas, aumenta la dificultad para obtener una visión general y actualizada de los proyectos.

* **La coordinación depende en gran medida de la comunicación:** El 66,6% utiliza WhatsApp como una herramienta importante para coordinar actividades. Esto demuestra que la comunicación es necesaria, pero también plantea una oportunidad para complementar los mensajes informales con información estructurada y trazable dentro de Vantage PMO.

* **Las alertas y recordatorios pueden reducir problemas de seguimiento:** El 66,6% considera útiles las alertas o recordatorios. Esta funcionalidad podría ayudar a los usuarios a controlar fechas importantes, tareas pendientes y posibles retrasos.

* **La facilidad de uso es una condición para la adopción:** El 100% de los entrevistados considera importante que la herramienta sea sencilla y práctica. Por ello, Vantage PMO debe buscar una experiencia intuitiva que permita incorporar la plataforma al flujo de trabajo sin requerir una capacitación extensa.

* **Existe una oportunidad para el acceso móvil:** Aunque solo el 33,3% menciona explícitamente el acceso desde dispositivos móviles, esta característica puede resultar útil para usuarios que necesitan consultar información mientras se encuentran fuera de su espacio habitual de trabajo.
## 2.3 Needfinding
<a id="2-3-needfinding"></a>

En esta sección se presentan los artefactos obtenidos a partir del análisis de las entrevistas realizadas a los segmentos objetivo de Vantage PMO. Estos artefactos permiten representar las necesidades, comportamientos, tareas, motivaciones y dificultades de los usuarios.

Para la construcción de los User Personas se consideraron los principales patrones identificados durante las entrevistas, complementándolos con el análisis competitivo realizado previamente. A partir de estos perfiles se elaboraron el User Task Matrix, los User Journey Maps y los Empathy Maps, buscando representar la situación actual de los usuarios antes de utilizar Vantage PMO.

### 2.3.1 User Personas
<a id="2-3-1-user-personas"></a>

Se elaboraron dos User Personas, uno por cada segmento objetivo identificado para Vantage PMO. Los perfiles representan los principales patrones encontrados durante el análisis de entrevistas y permiten comprender sus objetivos, necesidades, comportamientos y frustraciones.

**Segmento 1**

![User Persona Gerson](assets/images/Gerson%20Escarate.png)

El User Persona del segmento 1 representa a un líder o jefe de gestión de proyectos que debe supervisar múltiples proyectos de manera simultánea. Su principal necesidad es mantener una visión actualizada del estado de los proyectos y contar con información confiable para tomar decisiones oportunas.

El análisis de las entrevistas muestra que este perfil utiliza diferentes herramientas para realizar el seguimiento de sus proyectos y que una de sus principales dificultades está relacionada con la consolidación de información. Asimismo, requiere conocer el avance de las tareas, responsables, fechas y posibles desviaciones.

Su principal motivación es mejorar el control de los proyectos y reducir el tiempo dedicado a actividades administrativas, especialmente aquellas relacionadas con la recopilación y elaboración de reportes. Valora las herramientas que presentan información de manera clara, permiten identificar problemas oportunamente y son sencillas de utilizar.

**Segmento 2**

![User Persona Alessandro](assets/images/Alessandro%20Nieto.png)

El User Persona del segmento 2 representa a una persona que participa en una organización con múltiples proyectos o iniciativas y que necesita coordinar tareas, responsables y fechas entre diferentes personas.

Este perfil utiliza principalmente herramientas independientes como hojas de cálculo, servicios de almacenamiento y aplicaciones de comunicación. La información distribuida entre diferentes canales dificulta obtener una visión general del estado de los proyectos y mantener todos los datos actualizados.

Su principal motivación es mejorar la organización y coordinación del trabajo, evitando olvidos, retrasos y duplicidad de información. Valora especialmente una solución centralizada que sea sencilla de utilizar, requiera poca capacitación y facilite el seguimiento de las actividades.

---

### 2.3.2 User Task Matrix
<a id="2-3-2-user-task-matrix"></a>

El User Task Matrix permite identificar las principales tareas que realizan los User Personas para alcanzar sus objetivos, independientemente de la existencia de Vantage PMO. Para cada tarea se considera su frecuencia y nivel de importancia dentro de las actividades de cada segmento.

| Task | Líder / Jefe de Gestión de Proyectos |  | Empresas Medianas y Grandes con Múltiples Proyectos |  |
| :--- | :---: | :---: | :---: | :---: |
| | **Frecuencia** | **Importancia** | **Frecuencia** | **Importancia** |
| Revisar el estado de los proyectos | Diaria | Crítica | Diaria | Alta |
| Actualizar información de proyectos | Diaria | Alta | Diaria | Alta |
| Verificar tareas pendientes | Diaria | Alta | Diaria | Alta |
| Revisar fechas y plazos | Diaria | Crítica | Diaria | Crítica |
| Coordinar actividades con responsables | Diaria | Crítica | Diaria | Crítica |
| Identificar retrasos o desviaciones | Semanal | Crítica | Semanal | Alta |
| Consolidar información de diferentes fuentes | Semanal | Alta | Semanal | Alta |
| Elaborar o actualizar reportes | Semanal | Alta | Mensual | Alta |
| Revisar disponibilidad de recursos | Semanal | Alta | Semanal | Media |
| Comunicar avances a otros responsables | Diaria | Alta | Diaria | Alta |

El análisis de la matriz evidencia que ambos User Personas comparten tareas relacionadas con el seguimiento de proyectos, revisión de fechas, coordinación y actualización de información. Estas actividades presentan una frecuencia elevada debido a la necesidad de mantener el control sobre múltiples proyectos.

En el caso del líder o jefe de gestión de proyectos, las tareas relacionadas con la revisión del estado, identificación de desviaciones y elaboración de reportes presentan una importancia especialmente alta, debido a su responsabilidad en la toma de decisiones.

Por otro lado, el segundo User Persona presenta una mayor necesidad de coordinación y organización de tareas, debido al uso de diferentes herramientas y canales de comunicación. En ambos casos se identifica una oportunidad para centralizar información y facilitar el seguimiento de las actividades.

---

### 2.3.3 User Journey Mapping
<a id="2-3-3-user-journey-mapping"></a>

En esta sección se presentan los User Journey Maps en su estado actual (As-Is). Estos representan el recorrido que realizan los usuarios para gestionar y realizar el seguimiento de sus proyectos sin utilizar Vantage PMO.

Los mapas permiten visualizar las principales etapas del proceso, las acciones realizadas, los puntos de contacto utilizados y las dificultades que experimentan los usuarios. De esta manera, se identifican oportunidades de mejora relacionadas principalmente con la dispersión de información, el seguimiento de tareas y la coordinación entre responsables.

**Segmento 1**

![User Journey Map - Gerson Escarate](assets/images/User%20Journey%20Map%20-%20Gerson%20Escarate.png)

El recorrido del líder o jefe de gestión de proyectos inicia con la recopilación de información proveniente de diferentes responsables y herramientas. Posteriormente, revisa el avance de las tareas, verifica fechas y analiza posibles retrasos o desviaciones. Finalmente, consolida la información para comunicar el estado de los proyectos y elaborar reportes.

Durante este proceso puede experimentar dificultades debido a la información distribuida entre diferentes herramientas, la necesidad de actualizar datos manualmente y el tiempo requerido para consolidar reportes.

**Segmento 2**

![User Journey Map - Alessandro Nieto](assets/images/User%20Journey%20Map%20-%20Alessandro%20Nieto.png)

El recorrido del segundo User Persona comienza con la organización de las actividades y la asignación de tareas a los responsables. Posteriormente, realiza coordinaciones mediante diferentes canales de comunicación, verifica fechas y consulta el avance de las actividades.

Finalmente, recopila la información necesaria para conocer el estado de los proyectos. Durante este proceso pueden presentarse problemas relacionados con información dispersa, duplicidad de datos, falta de actualización y dificultad para realizar un seguimiento centralizado.

---

### 2.3.4 Empathy Mapping
<a id="2-3-4-empathy-mapping"></a>

Se elaboraron los Empathy Maps correspondientes a cada User Persona con el objetivo de profundizar en sus necesidades, comportamientos, pensamientos, emociones, frustraciones y motivaciones.

El análisis considera qué observa, escucha, dice y hace cada usuario, así como los principales Pains y Gains identificados a partir de las entrevistas. Esto permite comprender la experiencia actual de los usuarios y orientar las características de Vantage PMO hacia sus necesidades reales.

**Segmento 1**

![Empathy-Map-1](assets/images/chapter-2/Needfinding/Segment-1/Empathy-Map-Gerson-Escarate.png)

El líder o jefe de gestión de proyectos busca mantener el control de múltiples proyectos y disponer de información actualizada para tomar decisiones. Está expuesto constantemente a reportes, reuniones, mensajes y diferentes fuentes de información.

Entre sus principales Pains se encuentran la información dispersa, el tiempo dedicado a consolidar datos, la dificultad para identificar desviaciones y la necesidad de realizar seguimiento constante.

Sus principales Gains están relacionados con disponer de una visión general de los proyectos, reducir actividades administrativas, identificar problemas oportunamente y contar con información clara para tomar decisiones.

**Segmento 2**

![Empathy-Map-2](assets/images/chapter-2/Needfinding/Segment-2/Empathy-Map-Katherine-Herrera.png)

El segundo User Persona busca mantener organizadas las actividades de diferentes proyectos y coordinar correctamente a los responsables. Utiliza diferentes herramientas y canales para comunicarse y compartir información.

Entre sus principales Pains se encuentran la dispersión de información, la posibilidad de utilizar datos desactualizados, la duplicidad de información, los olvidos y las dificultades para realizar seguimiento.

Sus principales Gains están relacionados con centralizar la información, organizar las tareas y responsables, recibir recordatorios de actividades importantes y disponer de una herramienta sencilla que facilite la coordinación.

---

### 2.3.5 Big Picture EventStorming
<a id="2-3-5-big-picture-eventstorming"></a>

El Big Picture EventStorming permite representar de manera general los principales eventos que ocurren dentro del dominio de gestión de proyectos. A partir del análisis de los procesos actuales de los usuarios, se identificaron los eventos relacionados con el registro, planificación, seguimiento, coordinación y cierre de proyectos.

El objetivo es obtener una visión general del dominio antes de definir los componentes específicos de la solución.

**Eventos de dominio identificados:**

* *Project Registered:* Se registra un nuevo proyecto y se define la información inicial necesaria para su gestión.

* *Project Planned:* Se establecen las principales actividades, fechas y responsables asociados al proyecto.

* *Task Assigned:* Se asignan tareas a los responsables correspondientes.

* *Milestone Defined:* Se establecen hitos relevantes para controlar el avance del proyecto.

* *Resource Allocated:* Se asignan los recursos necesarios para ejecutar las actividades planificadas.

* *Project Progress Updated:* Se actualiza el avance de las actividades y del proyecto.

* *Project Delay Detected:* Se identifica un retraso o desviación respecto a la planificación establecida.

* *Information Consolidated:* Se recopila y consolida la información proveniente de los diferentes responsables.

* *Performance Report Generated:* Se genera un reporte con información relevante sobre el desempeño del proyecto.

* *Project Reviewed:* Los responsables revisan el estado general del proyecto y sus principales indicadores.

* *Strategic Decision Made:* Los responsables toman decisiones a partir de la información disponible sobre el proyecto.

---

### 2.3.6 Ubiquitous Language
<a id="2-3-6-ubiquitous-language"></a>

El Ubiquitous Language establece un lenguaje común para los conceptos principales del dominio de gestión de proyectos. Su objetivo es evitar ambigüedades y facilitar la comunicación entre los miembros del equipo y los stakeholders.

* *Project:* Iniciativa temporal organizada para alcanzar un objetivo específico mediante un conjunto de actividades y recursos.

* *Project Manager:* Profesional responsable de planificar, coordinar y supervisar la ejecución de un proyecto.

* *PMO (Project Management Office):* Área de la organización encargada de establecer y supervisar prácticas relacionadas con la gestión de proyectos.

* *Stakeholder:* Persona o grupo interesado o afectado por los resultados de un proyecto.

* *Portfolio:* Conjunto de proyectos y otras iniciativas gestionadas de manera conjunta para alcanzar objetivos estratégicos de la organización.

* *Task:* Actividad específica que debe realizarse para contribuir al cumplimiento de los objetivos de un proyecto.

* *Milestone:* Punto significativo dentro de un proyecto que representa el cumplimiento de un resultado o etapa importante.

* *Project Progress:* Estado de avance de un proyecto respecto a las actividades y objetivos planificados.

* *Resource:* Persona, presupuesto, material u otro elemento necesario para ejecutar las actividades de un proyecto.

* *Project Delay:* Situación en la que una actividad, hito o proyecto presenta un avance inferior al planificado y puede afectar sus fechas establecidas.

* *Performance Report:* Documento que presenta información relevante sobre el desempeño, avance y estado de un proyecto.

* *Project Status:* Situación actual de un proyecto considerando su avance, tareas, fechas, recursos y posibles desviaciones.

* *Information Silo:* Información aislada en diferentes fuentes o áreas que dificulta su acceso, actualización y utilización conjunta.

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
| **id** | bigint | N-N | default | Identificador único del registro, generalmente una clave primaria. |
| **created_at** | datetime | NULL | default | Fecha y hora en que se creó el registro. |
| **updated_at** | datetime | NULL | default | Fecha y hora de la última actualización del registro. |
| **company_name** | varchar | NULL | default | Nombre de la empresa asociada al usuario o entidad. |
| **email** | varchar | N-N | default | Dirección de correo electrónico del usuario. |
| **first_name** | varchar | N-N | default | Primer nombre del usuario. |
| **last_name** | varchar | N-N | default | Apellido del usuario. |
| **password** | varchar | N-N | default | Contraseña del usuario (almacenada de forma segura, usualmente encriptada). |
| **trial** | bit | NULL | default | Indica si el usuario está en un período de prueba (true/false)[. |
| **username** | varchar | N-N | default | Nombre de usuario único utilizado para iniciar sesión. |

**Tabla: USER_AUDITS**

| Campo | Tipo | Nulo | Default | Comentario / Descripción |
| :--- | :--- | :--- | :--- | :--- |
| **id** | bigint | N-N | default | Identificador único del registro de auditoría. |
| **user_id** | bigint | N-N | default | Clave foránea que referencia a la tabla USERS. |
| **action** | varchar | N-N | default | Descripción de la acción o evento realizado por el usuario. |
| **timestamp** | datetime | N-N | default | Fecha y hora exacta en la que se registró el evento de auditoría. |

