---
title: <span class="small">Data visualization</span>
pagetitle: Data visualization
subtitle: From micro to macro, with context
author: Mikel Madina & Miren Berasategi
theme: deusto
deusto: TRUE
slide-level: 3
...

## 1. Data visualization as artefact  {data-transition="slide-in fade-out"}

### {data-transition="fade-in slide-out"}

<h2>1. Data visualization as artefact</h2>

<blockquote markdown=1 style="font-size:.7em;font-style:normal;">
 
<span style="font-size:1.5em;">artefact </span> <small style="vertical-align:middle !important">(<em>US</em> <strong>artifact</strong>)</small> <small style="vertical-align:middle !important;font-weight:bold;color:green">noun</small></blockquote>

. . . 

<blockquote markdown=1 style="font-size:.7em;font-style:normal;">
<small>1</small> An object made by a human being, typically one of cultural or historical interest.  

<em>‘gold and silver artefacts’</em>
</blockquote>

. . .

<blockquote markdown=1 style="font-size:.7em;font-style:normal;">

<small>2</small> Something observed in a scientific investigation or experiment that is not naturally present but occurs as a result of the preparative or investigative procedure.

<em>‘the curvature of the surface is an artefact of the wide-angle view’</em>
</blockquote>

. . . 

<span class="source">The Oxford Dictionary of English</span>

### <span class="pretitle">1. Data visualization as artefact</span> The atomic level  {data-transition="slide-in fade-out"}

Number of observations &rarr; marks

. . .

<!-- Data Density
An overall characteristic of the visual elements, used in combination, is data density. Data density refers to the number of useful data points you can get into an area 

. . . --> 

<table style="margin:2em auto;font-family:'Fira Mono';background-color:#eee;">
    <tr>
        <td style="border-bottom:0 solid white;text-align:right;padding:0 1em;">data points</td>
        <td rowspan="2" style="vertical-align:middle;border-bottom:0 solid white;">  &lt; </td>
        <td rowspan="2" style="vertical-align:middle;border-bottom:0 solid white;"> pixels</td>
    </tr>
    <tr>
        <td style="text-align:right;padding:0 1em;">observations</td>
    </tr>
</table>

. . .

In a picture of 1000 x 1000 pixels, the maximum of observations to fit is 10<sup><small>6</small></sup> (1 million). How big is that?

### <span class="pretitle">1. Data visualization as artefact</span> The atomic level  {data-transition="fade"}

Some strategies to overcome these constraints:

>1. Filter
>2. Split data into multiple charts
>3. Augmenting visualizations
>4. Densify

### <span class="pretitle">1. Data visualization as artefact</span> The atomic level  {data-transition="fade"}

**1. Filter observations** <span class="trend"></span>

>- By design, communicating a selection of data
>- By allowing the user to filter according to their interests
>    + Innovative filtering <span class="innovation"></span> (i.e. [Smart brushing](https://youtu.be/VU117h6wT6w?t=576))

### {data-transition="fade" data-background-iframe="https://www.youtube.com/embed/VU117h6wT6w?controls=0&amp;start=576"}

### <span class="pretitle">1. Data visualization as artefact</span> The atomic level  {data-transition="fade"}

**2. Split data into multiple charts** <span class="trend"></span>

Facets, trellis, small multiples

### <span class="pretitle">1. Data visualization as artefact</span> The atomic level  {data-transition="fade"}

**2. Split data into multiple charts** <span class="trend"></span>

![Example facet visualization of the observation of animals<br/> by species and sex (Michonneau & Fournier 2018)](facets.png){height="325"}

### <span class="pretitle">1. Data visualization as artefact</span> The atomic level  {data-transition="fade"}

**2. Split data into multiple charts** <span class="trend"></span>

![Example of small multiples: The Trilogy Meter (Meth 2009)](smallmultiples2.jpg){height="350"}

::: notes

Small multiples are sets of charts of the same type, with the same scale, presented together at a small size and with minimal detail, usually in a grid of some kind. The term was at least popularized by Edward Tufte, appearing first in his Visual Display of Quantitative Information in 1983. He says of them:

    Small multiples are economical: once viewers understand the design of one [chart], they have immediate access to the data in all the other [charts]… as the eye moves from one [chart to the next, the consistency of the design allows viewers to focus on changes in the data rather than on changes in graphical design.

:::


### <span class="pretitle">1. Data visualization as artefact</span> The atomic level  {data-transition="fade"}

**3. Augmenting visualizations** <span class="trend"></span>

. . .

![[ggExtra](https://daattali.com/shiny/ggExtra-ggMarginal-demo/), adding marginal histograms to ggplot2 (by Dean Attali)](ggplot-extra.png){height="350"}

### <span class="pretitle">1. Data visualization as artefact</span> The atomic level  {data-transition="fade"}

**4. Densify**

>- Escaping overplotting in scatterplots <span class="trend"></span>

. . .

![Clearly overplotted scatterplot (Kovalyshyn 2017)](scatterplot1.png){height="325"}

### <span class="pretitle">1. Data visualization as artefact</span> The atomic level  {data-transition="fade"}

**4. Densify**

- Escaping overplotting in scatterplots <span class="trend"></span>

![Using transparency is not helpful (Kovalyshyn 2017)](scatterplot2.png){height="325"}

### <span class="pretitle">1. Data visualization as artefact</span> The atomic level  {data-transition="fade"}

**4. Densify**

- Escaping overplotting in scatterplots <span class="trend"></span>

![Now we can **see** density (Kovalyshyn 2017)](scatterplot-hexbin.png){height="325"}

### <span class="pretitle">1. Data visualization as artefact</span> The atomic level  {data-transition="fade"}

**4. Densify**

- Timelines <span class="innovation"></span>

step-by-step

![DenseLines, a density representation of many time series as a heatmap (Moritz & Fisher)](denselines.png){height="325"}

### <span class="pretitle">1. Data visualization as artefact</span> The atomic level  {data-transition="fade"}

Adding the time factor:

- Static visualizations with real data (at the time of loading)
- Real-time visualizations, static and auto-refreshed
- Streaming data visualizations showing the flow of data

Require an additional effort for operational intelligence, where immediate decision making could be a requirement.

<span class="source">Source: Aragues 2018</span>

::: notes

A static visualization that uses the data that is available when the visualization is created. Any new data requires a refresh.

A real-time visualization that looks like the static one but updates itself constantly.

A streaming data visualization that shows the flow of data and the impact it has on the statistics.

:::

### <span class="pretitle">1. Data visualization as artefact</span> The atomic level  {data-transition="fade"}

How to communicate _nothingness_? (Kirk 2014)

###  {data-transition="fade" data-background-iframe="https://www.youtube.com/embed/JqzAuqNPYVM?start=524"}

### <span class="pretitle">1. Data visualization as artefact</span> The atomic level  {data-transition="fade"}

How to communicate _nothingness_?

>- **Null** &nbsp; Absence of measurement
>- **Zero** &nbsp; Absence of amount/magnitude
>- **Blank** &nbsp; Try to use _nothing_ to represent _something_

::: notes

`null` in the age of information overload, data absence is more and more significant
`zero` can be represented by 

- position + axis
- area + axis
- color shading
- density
- angle? we can't see 0º
- area only? we can't see

the last two require an alternative (like annotation)

`blank` gives us space to breath. requires courage, implies losing the potential to densify, add advertising

:::

###  {data-transition="fade" data-background-iframe="https://www.youtube.com/embed/JqzAuqNPYVM?start=1153"}

### <span class="pretitle">1. Data visualization as artefact</span> The atomic level  {data-transition="fade"}

How to communicate _nothingness_?

- **Null** &nbsp; Absence of measurement
- **Zero** &nbsp; Absence of amount/magnitude
- **Blank** &nbsp; Try to use _nothing_ to represent _something_

>- The design should be **invisible**

###  {data-transition="fade" data-background-iframe="https://www.youtube.com/embed/JqzAuqNPYVM?start=1363"}

### <span class="pretitle">1. Data visualization as artefact</span> The atomic level {data-transition="fade-in slide-out"}

Projections, statistical models, uncertainty

Unpublished papers:

<span class="source left">Alex Kale, Francis Nguyen, Matthew Kay, Jessica Hullman (2019), "[Hypothetical Outcome Plots Help Untrained Observers Judge Trends in Ambiguous Data](https://idl.cs.washington.edu/papers/hops-trends/)", _IEEE Trans. Visualization & Comp. Graphics (Proc. InfoVis)_, 2019</span>

### <span class="pretitle">1. Data visualization as artefact</span> Number of variables 

- Reduce dimensionality (statistically): PCA, factors, clusters
- Restructure dataset (from wide to tall) (heatmaps)

### <span class="pretitle">1. Data visualization as artefact</span> Generating a new language <span class="innovation"></span> {data-transition="slide-in fade-out"}

A word of caution:

- will need to be custom coded
- readers will require training
- correct interpretation may be more time demanding

. . . 

[Xenographics](https://www.xeno.graphics/): Weird <span class="fragment">but (sometimes) useful </span>charts

### <span class="pretitle">1. Data visualization as artefact</span> Generating a new language <span class="innovation"></span> {data-transition="fade"}

![Horizon charts](horizonchart.png)
  
<span class="source">Source: Jeffrey Heer, Nicholas Kong, Maneesh Agrawala (2009), "[Sizing the Horizon: The Effects of Chart Size and Layering on the Graphical Perception of Time Series Visualizations](http://vis.berkeley.edu/papers/horizon/)". _ACM Human Factors in Computing Systems (CHI)_, pp. 1303 - 1312</span>

### <span class="pretitle">1. Data visualization as artefact</span> Generating a new language <span class="innovation"></span> {data-transition="fade"}

![Choropleth maps with `tricolore`](tricolore.png){height="325"
}
 
<span class="source">Source: Jonas Schöley (2018), "[Choropleth maps with tricolore](https://cran.r-project.org/web/packages/tricolore/vignettes/choropleth_maps_with_tricolore.html)"</span>

### <span class="pretitle">1. Data visualization as artefact</span> Generating a new language <span class="innovation"></span> {data-transition="fade"}

![Flame graphs](flamegraph.svg){height="325"
}
 
<span class="source">Source: Brendan Gregg (2016), "[The Flame Graph](https://queue.acm.org/detail.cfm?id=2927301)". _ACM Queue_ Vol. 14, No. 2</span>

### {data-background-image="flamegraph.svg" data-transition="fade-in slide-out"}

### <span class="pretitle">1. Data visualization as artefact</span> Multiple Linked Views (MLV) <span class="trend"></span> <span class="innovation"></span> {data-transition="slide-in fade-out"}

_Making Data Visual_

<span class="source">
Ricardo Langner, Ulrike Kister, Raimund Dachselt (2019). "[Multiple Coordinated Views at Large Displays for Multiple Users: Empirical Findings on User Behavior, Movements, and Distances](https://imld.de/en/research/research-projects/mcv-displaywall/)", _IEEE Transactions on Visualization and Computer Graphics_ 25(1) (InfoVis 2018, Berlin) [`10.1109/TVCG.2018.2865235`](https://doi.org/10.1109/TVCG.2018.2865235)</span>

### {data-background-iframe="https://www.youtube.com/embed/kiXMn2VPZek" data-transition="fade-in slide-out"}

### <span class="pretitle">1. Data visualization as artefact</span> Beyond 2 dimensions <span class="innovation"></span> {data-transition="slide-in fade-out"}

### {data-background-iframe="https://www.youtube.com/embed/8j9r9JKIqww" data-transition="fade"}

<!--
    Realidad virtual:
    Still purely graphic, tú te metes en el gráfico.
-->

### {data-background-iframe="https://www.youtube.com/embed/p4fB_OfoaZA" data-transition="fade"}


<!-- Realidad aumentada:
    El gráfico se saca a la realidad y se coordina con elementos de la realidad física.
-->

### <span class="pretitle">1. Data visualization as artefact</span> Beyond 2 dimensions <span class="innovation"></span> {data-transition="fade-in slide-out"}


- Virtual Reality
- Augmented reality

References:

<span class="source left">
Ronell Sicat, Jiabao Li. [_DXR: A Toolkit for Building Immersive Data Visualizations_](https://sites.google.com/view/dxr-vis/download?authuser=0)
</span>

<span class="source left">
Christophe Hurter, Nathalie Henry Riche, Steven M. Drucker, Maxime Cordeil, Richard Alligier, Romain Vuillemot (2018), "[FiberClay: Sculpting Three Dimensional Trajectories to Reveal Structural Insights](http://recherche.enac.fr/~hurter/FiberClay.html)", IEEE Transactions on Visualization and Computer Graphics_ 25(1) (InfoVis 2018, Berlin)</span>

### <span class="pretitle">1. Data visualization as artefact</span> Senses and control interfaces <span class="innovation"></span>

(How is this _visualization_?)

- Wheeled micro robots
- Sound
- _smell necklace_ https://twitter.com/NElmqvist/status/1055370456528773120

## 2. Data visualization as a tool for communication {data-transition="slide-in fade-out"}

### {data-transition="fade"}

<h2 style="margin-bottom:2em;">2.&nbsp;Data visualization as a tool for communication</h2>

>The modern approach to data visualization is focused on quickly making data visualization. 

<span class="source">(Meeks 2018)</span>

### {data-transition="fade"}

<h2>2.&nbsp;Data visualization as a tool for communication</h2>

Focus on speed affects:

- how data visualization products are designed
- what tools are used to create them
- the role of the creator in relation to the product
- how engagement with readers in envisioned

::: notes

>This breackneck pace is a real data visualization constraint.

The fast mode of dataviz is real and important, but when we let it become our only view into what dataviz is, we limit ourselves in planning for how to build, support and design dataviz.

:::

### {data-transition="fade-in slide-out"}

<h2 style="margin-bottom:1em;">2.&nbsp;Data visualization as a tool for communication</h2>

>Ultimately, data visualization is not a technical problem, it's a design problem and, more than that, <span class="highlighted">a communication problem</span>.

<span class="source">(Meeks 2018)</span>

. . .

Let's look at what charts <span class="fragment">**say**</span><span class="fragment">, **mean**</span><span class="fragment">, and **do**.</span>

::: notes

Let's go slow down a bit

:::


### <span class="pretitle">2. Data visualization as a tool for communication</span> What charts say {data-transition="slide-in fade-out"}

**Explicitly**

Charts _do_ "show me the data" (but remember that it's more that they **tell** the data than actually show it).

Means chosing the right specific chart to use in order to display and query the data.

. . .

**How to improve:** Expose data cleanly and clearly. Accuracy _vs._ precision.

::: notes

Accuracy refers to the closeness of a measured value to a standard or known value. For example, if in lab you obtain a weight measurement of 3.2 kg for a given substance, but the actual or known weight is 10 kg, then your measurement is not accurate. In this case, your measurement is not close to the known value.

Precision refers to the closeness of two or more measurements to each other. Using the example above, if you weigh a given substance five times, and get 3.2 kg each time, then your measurement is very precise. Precision is independent of accuracy. You can be very precise but inaccurate, as described above. You can also be accurate but imprecise.

For example, if on average, your measurements for a given substance are close to the known value, but the measurements are far from each other, then you have accuracy without precision.

::: 

### <span class="pretitle">2. Data visualization as a tool for communication</span> What charts say {data-transition="fade"}

**Implicitly**

No chart is an unbiased view of the data, as data visualization is a manufactured artefact.

<blockquote style="font-size:.8em">
    
    All data is transformed to be in a chart, and the inaction of not designing that transformation carries just as strong an implication as the action of transforming it.

</blockquote>

<span class="source">(Meeks 2018)</span>

### <span class="pretitle">2. Data visualization as a tool for communication</span> What charts say {data-transition="fade"}

<table style="margin-top:-25px;">
    <tr>
        <td>
        ![Most _default_ representation of an histogram](iraq-redesigned.png){height="450"}
        </td>
        <td class="fragment">![Original infographic by Simon Scarr (Meeks 2018)](iraq.png){height="450"}</td>
    </tr>
</table>

<figure class="fragment"><figcaption>
Original infographic (right) by Simon Scarr and redesigned, more default representation of an histogram (left), redesigned by Andy Cotgreave (Meeks 2018)</figcaption></figure>

::: notes

Very strong message. Red, bars point down, looks like blood. Very evocative, emphasized by the title.

Rotation: There's still a peak, but the decline is more apparent

Title: To match the main takeaway of the graph

Color: not like blood anymore

"Situation in Iraq is improving" --> Completely different message!

Neither of those charts is lying. The opinionated nature of charts should be acknowledged and embraced. 

:::

### <span class="pretitle">2. Data visualization as a tool for communication</span> What charts say {data-transition="fade"}

**Implicitly**

The implicit channel of a data visualization (the title and other framing elements) can be even more powerful than the explicit channel.

. . .

**How to improve:** Style should be intentional, purposeful and thematically appropriate, not the result of defaults or superficial decisions.

### <span class="pretitle">2. Data visualization as a tool for communication</span> What charts say {data-transition="fade"}

**Systematically** 

<br />

>[...] all charts display data and all data is a proxy for the systems that created and measured that data.

<span class="source">(Meeks 2018)</span>

. . .

**How to improve:** Caution not to reveal an underlying system that is proprietary or confidential.

::: notes

There's sort of a cruel irony to the way we simultaneously share these data products so enthusisastically while bemoaning the privacy issues that are necessary for their creation.

:::

### <span class="pretitle">2. Data visualization as a tool for communication</span> What charts say {data-transition="fade"}

**Descriptively**

>- internally: axes, labels, annotations
>- externally: surrounding text, figure descriptions, discussions

. . .

Unlike the implicit channel, the descriptive channel is active and purposeful (not subconscious).

. . .

**How to improve:** Consider annotations, labels, axis elements as part of the data visualization.

### <span class="pretitle">2. Data visualization as a tool for communication</span> What charts say {data-transition="fade-in slide-out"}

>By being more explicit in our own understanding of what charts say and how we can systematically describe what they say, we can grow more capable of using the channels available in that expression to our advantage.

<span class="source">(Meeks 2018)</span>

. . .

What does your chart say that you didn't intend?

### <span class="pretitle">2. Data visualization as a tool for communication</span> What charts mean {data-transition="slide-in fade-out"}

Charts mean more than just what they say.

### <span class="pretitle">2. Data visualization as a tool for communication</span> What charts mean {data-transition="fade"}

**Intentionally**

>The mode and purpose of a chart should be well understood by the chart maker and immediately apparent to the chart reader.

<span class="source">(Meeks 2018)</span>

### <span class="pretitle">2. Data visualization as a tool for communication</span> What charts mean {data-transition="fade"}

**Historically**

Charts are products of their time. 

It is important to provide background about the data sources, to enable checking whether they are still based on relevant priorities, dimensions and metrics.

### <span class="pretitle">2. Data visualization as a tool for communication</span> What charts mean {data-transition="fade"}

**Historically**

![Obesity chart](obesity.png)

### <span class="pretitle">2. Data visualization as a tool for communication</span> What charts mean {data-transition="fade"}

**Culturally**

Charts should be adapted to the culture they will be consumed in (think user-centered design techniques).

### <span class="pretitle">2. Data visualization as a tool for communication</span> What charts mean {data-transition="fade"}

**Contextually**

Enable removing and adjusting data visualization elements to reduce complexity, not based on screen size as in responsive data visualization, but on priority.

### <span class="pretitle">2. Data visualization as a tool for communication</span> What charts mean {data-transition="fade-in slide-out"}

>Meaning-making may sound too soft to the kind of technical professionals that make and read data visualization but communication without meaning is just noise.

<span class="source">(Meeks 2018)</span>

### <span class="pretitle">2. Data visualization as a tool for communication</span> What charts do {data-transition="slide-in fade-out"}

The most important thing about a chart is its impact. 

### <span class="pretitle">2. Data visualization as a tool for communication</span> What charts do {data-transition="fade"}

**Provide insights**

Identify and emphasize the insights that the readers might expect

![simple line chart and highlighted features of the line chart](insight.png)

### <span class="pretitle">2. Data visualization as a tool for communication</span> What charts do {data-transition="fade"}

**Cause change**

As difficult to measure as it is important.

How have they impacted business decisions? How were they used in presentations? Where they modified (changed colours, cropped, annotated) somehow?

::: notes

Understanding how a particular chart was an effective piece of evidence or motivation is key to developing more effective data visualization.

:::

### <span class="pretitle">2. Data visualization as a tool for communication</span> What charts do {data-transition="fade"}

**Cause visual literacy**

>All data visualization was, at some point, complex data visualization, until an audience grew comfortable and literate enough to read it.

<span class="source">(Meeks 2018)</span>

(Netflix connected scatterplot chart?)

::: notes

Languages are live things, that evolve over time, and require breakthrough.

>[...] the new form cannot be introduced until it is understood but can only be understood once it's introduced.

:::

### <span class="pretitle">2. Data visualization as a tool for communication</span> What charts do {data-transition="fade"}

**Create new charts**

![Imaginary genealogy for charts with scatterplots as a common ancestor (Meeks 2018)](chartlineage.png)

::: notes

Catalogs of data visualization have the tendency to treat every form as a category of one without drawing connections between them, which disguises how charts lead to other charts.

:::

### <span class="pretitle">2. Data visualization as a tool for communication</span> What charts do {data-transition="fade-in slide-out"}

<br />

>All communication is evaluated based on content, but presuasive communication, which is all data visualization unless it is purely decorative, is rightly also evaluated based on effect.

<span class="source">(Meeks 2018)</span>

::: notes

Ultimately, what charts do may be the one most important thing.

:::

## 3. The artefact goes social

### <span class="pretitle">3. The artefact goes social</span> Data counseling {data-transition="slide-in fade-out"}

<br />

>[...] brings domain expertise into the operationalization process to help inform decisions about good proxies as well as to uncover insights using the resulting visualizations.

<span class="source">(Meyer & Fisher 2018)</span>


### <span class="pretitle">3. The artefact goes social</span> Data counseling {data-transition="fade"}

Based on **interviews** (1) for

>- gaining an understanding of the questions and data
>- get feedback on proxies, **explorations** (2), and visualization **prototypes** (3)

### <span class="pretitle">3. The artefact goes social</span> Data counseling {data-transition="fade"}

**1. Interviews**

>The role of the interviewer is to ask questions that will guide the stakeholders toward elucidating the information necessary for working through an operationalization process and designing visualizations.

<span class="source">(Meyer & Fisher 2018)</span>

### <span class="pretitle">3. The artefact goes social</span> Data counseling {data-transition="fade"}

**1. Interviews**

Identify stakeholders:

>- analysts
>- data producers
>- gatekeepers
>- decision makers
>- connectors

### <span class="pretitle">3. The artefact goes social</span> Data counseling {data-transition="fade"}

**1. Interviews**

Require practice and experience.

Semistructured: be prepared, but also be open.

>- start with open ended questions (problem, data, context)
>- use the conversation to search out the more abstract question

::: notes

unstructured: can uncover unknown needs and goals, but it can take a significant amount of time to get to anything useful.

structured: while efficient, leave little room for discovering new insights.

:::

### <span class="pretitle">3. The artefact goes social</span> Data counseling {data-transition="fade"}

**1. Interviews**

Use traditional conversation / interpersonal communication skills to prevent dead ends: keep them talking

>- rephrase responses back to the stakeholder
>- ask the same or similar questions in different ways
>- explore a completely different conversational topic

### <span class="pretitle">3. The artefact goes social</span> Data counseling {data-transition="fade"}

**1. Interviews**

Contextual interviews

>- take place in the stakeholder's work environment
>- consist of demonstrations of the tools and data inspection methods currently in use

::: notes

often starts by asking the stakeholder to either walk through a specific analysis task they have already performed or conduct someof their work for that day with the interviewer present. The stakeholder talks through each step they are taking.

:::

### <span class="pretitle">3. The artefact goes social</span> Data counseling {data-transition="fade"}

**2. Data exploration**

Look to the data as early as possible.

???

### <span class="pretitle">3. The artefact goes social</span> Data counseling {data-transition="fade"}

**3. Rapid prototyping**

>[...] is a process of trying out many visualization ideas as quickly as possible and getting feedback from stakeholders on their efficacy.

<span class="source">(Meyer & Fisher 2018)</span>

### <span class="pretitle">3. The artefact goes social</span> Data counseling {data-transition="fade"}

**3. Rapid prototyping**

&ne; _fast_ data visualization

&ap; agile/lean methodologies and user-centered design

### <span class="pretitle">3. The artefact goes social</span> Data counseling {data-transition="fade"}

**3. Rapid prototyping**

![Prototypes range from low-fidelity sketches to high-fidelity working models (Meyer & Fisher 2018)](prototypes.png)

::: notes

low-fi: sketched on paper or on a whiteboard, digital mockups that may include some controls for explaining interaction ideas (slides). Can incorporate charts generated in Excel or Tableau with fake or sampled data. Great for communicatingthe gist of an idea in an interview, fast and easy to produce. Rapidly establish whether the visualizationd designer is on the same page as the stakeholders.

hi-fi: custom visualizations which must be created from scratch. Largely contain the core functionality. Meant to be thrown away, the point is not to worry about the code other than to confirm that ideas can work.

:::

### <span class="pretitle">3. The artefact goes social</span> Data counseling {data-transition="fade"}

**3. Rapid prototyping**

Prototypes are made to obtain feedback on them: get to the stakeholders early and often.

Focus not on whether they like it or not, but rather on **what the visualization can and cannot do** (contextual interview where the stakeholder uses the visualization).

### Responsive data visualization

Data served

### Responsive data visualization

Device dependant

### Responsive data visualization

Alerts

## Epilogue

### Resources

http://oavis.steveharoz.com/

### References


<div class="source">

Ihor Kovalyshyn (2017), [_When Scatter Plot Doesn't Work_](https://delta1epsilon.github.io/2017/When-Scatter-Plot-doesn%27t-work/)

Dominik Moritz and Danyel Fisher (2018), "Visualizing a Million Time Serieswith the Density Line Chart" [ arXiv:1808.06019v2](https://arxiv.org/pdf/1808.06019.pdf) [cs.HC]

Andy Kirk 2014 Null zero blank

François Michonneau & Auriel Fournier (2018), “Data Carpentry: R for data analysis and visualization of Ecological Data.” doi: 10.5281/zenodo.569338, http://datacarpentry.org/R-ecology-lesson/

Dan Meth (2009), "The Trilogy Meter" https://danmeth.myportfolio.com//post/77471620/my-trilogy-meter-1-in-a-series-of-pop-cultural

Anthony Aragues (2018), _Visualizing Streaming Data_. O'Reilly Media

Miriah Meyer & Danyel Fisher (2018), _Making Data Visual_. O'Reilly Media

</div>

### Thank you!