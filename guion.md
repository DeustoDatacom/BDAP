# Data visualization 

## 1 Notas sobre el grupo

De 16 _startups_, 5 mencionan que van a usar visualizaciones:

- 3 de robotica (VW)
- 2 energía (HVAC: Heating, Ventilation and Air Conditioned)

## 2 Posible título

**Data visualization: from micro to macro (and it’s context)**

Micro sería cada una de las observaciones, Macro sería MLV (multiple linked views).

Lo del contexto sería la parte más comunicativo-cultural (Elijah Meeks)

## 3 Partes
### 3.1 La visualización de datos como artefacto

**Graphic constraints** (especialmente agudizado en el caso de Big Data, pero no exclusivo)

- Number of observations/marks…
    - Filter
    - Trellis
    - Densify (de momento la normal, luego la de timmelines)
    - Algo sobre real time
        - En gráficas basadas en tiempo (timeline) puede, pero en otras puede despistar (y mucho)
    - ¿Y los datos que no existen?
    - Algo sobre zeno/null/NaN
    - Proyecciones: Algo sobre modelos estadísticos: uncertainty…
- Number of variables
    - Reducir dimnesionalidad (estadísticamente)
    - Reestructurar dataset from wide to tall Convertir variables en niveles de un factor, bla bla bla
- A nivel de gráfica: Xenographics: tenemos que ir más allá? Hay que inventar nuevas gráficas?
    - pros y contras (casi seguro habrá que codificarlo, y además training para el usuario, su interpretación correcta requiere de más tiempo)
    - Xenographics https://xeno.graphics/
        - Horizon charts / cubism.js (http://square.github.io/cubism/ horizon chart)
        - mapas tricolores (https://cran.r-project.org/web/packages/tricolore/vignettes/choropleth_maps_with_tricolore.html)
            - Flamegraphs http://www.brendangregg.com/flamegraphs.html -MLV (normalmente no trabajaremos con una sola gráfica)
        (revisar capitulito de Making data visual)

### 3.2 La visualización de datos en su contexto social (herramienta de comunicación)

Elijah Meeks What charts [Say](https://medium.com/@Elijah_Meeks/what-charts-say-6e31cbba2047), [Mean](https://medium.com/@Elijah_Meeks/what-charts-mean-a4f790bb3c89), [Do](https://medium.com/@Elijah_Meeks/what-charts-do-48ed96f70a74)

#### 3.2.1 Say

- **Implicitly**: Charts should be distinctive if their dataset is distinctive or stylistically related if the data/view is related. Above all style should be intentional, purposeful and thematically appropriate. Titles, colors and other graphical design elements should have well-reasoned justification for their choices and not be the result of defaults or superficial decisions.
- **Systematically**: Care should be taken not to reveal an underlying system that is proprietary or confidential. Data provenance should be as close to the chart as possible (either through notes or charts). Systems should influence the design and iteration process as avenues of exploration (chart inversion, multimodal network projection). In cases where a data visualization is for the purpose of understanding a system, strive to represent that system rather than the easier to measure proxies of that system. This means more network diagrams and fewer bar charts.
- **Descriptively**: Annotations should be present whenever possible, and preferred over interactivity, which is spotty. Labels should be descriptive and aware of how they magnify or occlude the data. Axis elements should be treated as data visualization and open to interactivity, robust styling and smart labels.
- What does your chart say that you didn’t intend?

#### 3.2.2 Mean

- **Intentionally**: The mode and purpose of a chart should be well-understood by the chart maker and immediately apparent to the chart reader. If it’s one of many views from a data dashboard then make sure at a glance that the key messages are clear via distinctive but tidy labels and annotations. If it’s a figure in a presentation, use graphics to highlight where you want your audience to look and text to summarize why they’re looking at this graphic.
- **Historically**: As a reader, always ask if the charts and dashboards you’re using are still based on relevant priorities, dimensions and metrics. As a chart creator, try to keep track of where your charts are in use and make sure that dashboards are refreshed to reflect changes in organizational focus. This is one reason why it’s important to show data sources on charts so that future readers can properly make use of them.
- **Culturally**: When making data visualization make sure you have a clear idea of the audiences for your charts using traditional techniques of user-centered design like personas and interviews. Decision makers should recognize the investment necessary to make broadly accessible data visualization and consider its impact and value for recruiting and connecting disparate units.
- **Contextually**: If you can, design and provide a contextual version of the chart that is suitable for inclusion alongside other charts. Similar to responsive design of charts, contextual design focuses on removing and adjusting data visualization elements to reduce complexity only in the case of context this is based on priority instead of screen size. This can be done by desaturating the colors, reducing the number of dimensions or, more crudely, by obviously labeling it in a way to signal it is context. A chart that’s being integrated into another display or presentation can find itself in front of an audience that does not have the same domain knowledge as the primary audience, so this is yet another reason to have its data sources, dimensions and metrics more explicitly described.

    > Meaning what you make

#### 3.2.3 Do

- **Reveal Insights**: Understand the kinds of insights that your readers are looking for. Be able to categorize those insights and describe, graphically, how they appear in the data visualization products you create. Focus on and describe the methods you’re using to help your readers identify, collect and deploy those insights. Evaluate the data visualization methods you’re using to determine how they improve and hold back the creation and collection of these insights.
- **Cause Change**: Track and measure the impact of charts on business decisions via interviews and examples of how charts have been used in presentations and memos. Be aware of how charts are used and whether they are used in their original form in the applications where they’re deployed or whether they’re used as screenshots or with graphical modification (like color changes, cropping, or notes). Identify when charts have had negative effects due to confusion or misunderstanding. Make sure decision makers recognize the role of charts in their decisions.
- **Cause Visual Literacy**: Keep track of how your choices of data visualization method are constrained by the visual literacy of your audience. Try to find areas where the insights your readers expect can be improved with a chart that they are not comfortable with and introduce it to them. Track what works and what doesn’t as far as methods of teaching readers how to understand new charts.
- **Create New Charts**: Try to maintain a lineage of charts and views in your organization. Look at charts in use from external vendors to see if there are forms that are not commonly in use internally. External vendor tools often by virtue of being sales-focused tend to have more flamboyant and complex methods, which can be used to spur internal tools to adopt those methods. Keep an eye out for when particular stakeholders associate a certain chart with a certain perspective or dataset. Flame graphs, for instance, are often thought to only apply to processes on servers or rendering but the method they use, the partition layout, is generic and suitable for a wider range of applications.

[volvemos a xenographics]

### 3.3 Arrejuntando las dos (visualización como artefacto, pero teniendo en cuenta el aspecto social)
#### 3.3.1 Data counseling
#### 3.3.2 Responsive data visualization

Dispositivos:

- Resolución
- Colores
- Formas (circular)

Algo de dashboards ()

Alertas

- No solo gráficas
- Email / push
- Sonido (sirena)

