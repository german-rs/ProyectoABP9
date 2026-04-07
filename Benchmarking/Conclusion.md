# Benchmarking de LLMs sobre el ABP9: ¿Quién resuelve mejor un caso de narrativa de datos?

Como ejercicio paralelo al desarrollo del Proyecto ABP9 (*Diagnóstico y Comunicación de Insights Organizacionales*, Módulo 9 de Alkemy), se diseñó un benchmarking informal en el que la consigna completa fue presentada de forma idéntica a cinco modelos de lenguaje: **Claude**, **Gemini**, **ChatGPT**, **DeepSeek** y **Copilot**. El caso exigía identificar un insight sobre la caída de rendimiento de equipos internos en una empresa de tecnología, estructurarlo bajo el esquema Contexto–Problema–Hallazgo–Recomendación, justificar la estructura de datos seleccionada y proponer una visualización perceptivamente efectiva.

Las cinco respuestas fueron analizadas con **NotebookLM**, que evaluó el desempeño en las cuatro dimensiones del proyecto: profundidad analítica, estructura narrativa, rigor en el modelado de datos y calidad en la visualización. El resultado posicionó a **Claude** como el modelo con mejor desempeño integral: fue el único que simuló datos concretos con grupo de control —identificando que Soporte se mantuvo estable mientras Desarrollo y QA caían— para aislar la causa raíz, justificó técnicamente la elección del gráfico de líneas múltiples sobre alternativas como barras, y aplicó de forma explícita los principios de percepción visual requeridos en el manual del proyecto.

Tras un análisis exhaustivo de los requerimientos técnicos y pedagógicos detallados en el documento **"Proyecto_ABP9.pdf"**, he determinado que la respuesta proporcionada por **Claude** es la más completa, técnica y alineada con los objetivos del caso.

A continuación, presento los argumentos que sustentan esta decisión desde la perspectiva de un experto en análisis de datos:

### 1. Profundidad en el Análisis (Lección 1)
Mientras que otros modelos se limitaron a describir el problema, **Claude simuló un conjunto de datos específico** (una tabla de rendimiento porcentual de Q1 a Q4) para respaldar su diagnóstico. Lo más destacado es el uso de un **"grupo de control"**: al mostrar que el equipo de Soporte se mantuvo estable mientras Desarrollo y QA caían, el análisis logra aislar la causa raíz, cumpliendo con el objetivo de realizar un diagnóstico efectivo.

### 2. Estructura Narrativa y Storytelling (Lección 2)
Claude es el modelo que mejor aplica la **narrativa estructurada** solicitada (Contexto – Problema – Hallazgo – Recomendación). Su storyboard de 4 cuadros es claro, directo y está diseñado para una audiencia organizacional, permitiendo que un directivo comprenda el escenario y actúe en consecuencia.

### 3. Rigor en la Estructura de Datos (Lección 3)
El modelo identifica con precisión la **naturaleza de las variables** (temporales, cuantitativas continuas y cualitativas nominales). Además, justifica técnicamente la elección de un gráfico de líneas múltiples sobre otras opciones como las barras, explicando que la prioridad es comunicar una **tendencia de caída** y no solo valores puntuales.

### 4. Excelencia en Visualización de Datos (Lección 4)
Claude sobresale al aplicar explícitamente los **principios de percepción visual** requeridos en el manual del proyecto:
*   **Limpieza de ruido visual:** Elimina grillas innecesarias.
*   **Foco en lo importante:** Propone el uso de colores (rojo para Desarrollo) para dirigir la atención al insight.
*   **Marcas visuales:** Define correctamente el uso de posición, color y forma.
*   Incluso proporciona un **bosquejo ASCII del gráfico** y un título accionable que resume el hallazgo de inmediato.

### Comparativa con los demás modelos:
*   **Gemini** y **DeepSeek** presentaron respuestas sólidas y buenos insights (como el "tiempo de espera" o el "exceso de reuniones"), pero carecieron del nivel de detalle técnico en la justificación de la estructura de datos y los principios de diseño que Claude sí incluyó.
*   **ChatGPT** ofreció una respuesta correcta pero más genérica, sin profundizar en la simulación de datos.
*   **Copilot** fue el desempeño más bajo, ya que se limitó a resumir la consigna del proyecto sin resolver el caso práctico ni proponer un insight real.

**Conclusión:** Claude no solo cumple con los entregables, sino que demuestra una capacidad superior para **transformar datos en una historia comprensible y accionable**, alineándose perfectamente con la solicitud de la Dirección de Planificación Estratégica.