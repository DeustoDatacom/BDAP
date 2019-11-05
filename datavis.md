---
title: Data visualisation
pagetitle: Data visualisation
subtitle: from a communication perspective
date: <span style="display:block;margin-top:-1em;margin-bottom:1em;font-size:.8em;font-style:normal;">with Mikel Madina</span><span style="font-style:normal;">European Data Incubator</span><br />Bilbao, 6<small>th</small> November 2019
author: Miren Berasategi
theme: deusto
deusto: TRUE
...

### 

<div style="font-family:'Roboto';font-size:.6em;margin-top:2em;">


1. <span style="font-size:1.3em;">Data visualisation as an artefact</span>
    + The atomic level
    + Number of variables
    + Generating new idioms
    + Multiple Linked Views
    + Beyond 2 dimensions
    + Other senses
2.  <div style="font-size:1.3em;padding-top:.5em;">Data visualisation as a communication product</div>
    + What charts say
    + What charts mean
    + What charts do
3. <div style="font-size:1.3em;padding-top:.5em;">The artefact goes social</div>
    + Data counseling
    + Responsive data visualisation

</div>

# 1. Data visualisation <br />as an artefact  {data-transition="slide-in fade-out"}

### {data-transition="fade-in slide-out"}


<blockquote markdown=1 style="font-size:.7em;font-style:normal;margin-top:3em;">
 
<span style="font-size:1.5em;">artefact </span> <small style="vertical-align:middle !important">(<em>US</em> <strong>artifact</strong>)</small> <small style="vertical-align:middle !important;font-weight:bold;color:green">noun</small></blockquote>

<blockquote markdown=1 style="font-size:.7em;font-style:normal;">
<small>1</small> An object made by a human being, typically one of cultural or historical interest.  

<em>‘gold and silver artefacts’</em>
</blockquote>

<blockquote markdown=1 style="font-size:.7em;font-style:normal;">

<small>2</small> Something observed in a scientific investigation or experiment that is not naturally present but occurs as a result of the preparative or investigative procedure.

<em>‘the curvature of the surface is an artefact of the wide-angle view’</em>
</blockquote>

<span class="source">The Oxford Dictionary of English</span>

### <span class="pretitle">1. Data visualisation as an artefact</span> The atomic level  {data-transition="slide-in fade-out"}

  <br />

Maximum data density is `1:1`, and this is not usually the case:

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

::: notes

**Observations** need to be transformed into visual **marks**.

Data Density
An overall characteristic of the visual elements, used in combination, is data density. Data density refers to the number of useful data points you can get into an area.

In a picture of 1000 x 1000 pixels, the maximum of observations to fit is 10<sup><small>6</small></sup> (1 million). How big is that?

More than 1 pixel is used to represent each data point, + complimentary pixels for titles, labels, white space.

:::

### <span class="pretitle">1. Data visualisation as an artefact</span> The atomic level  {data-transition="fade"}

<br />

Some strategies to overcome this constraint:

>1. Filter observations
>2. Split data into multiple charts
>3. Augmenting visualisations
>4. Densify

### <span class="pretitle">1. Data visualisation as an artefact</span> The atomic level  {data-transition="fade"}

**1. Filter observations** <span class="trend"></span>

>- By design, communicating a selection of data
>- By allowing the user to filter according to their interests
>    + Innovative filtering <span class="innovation"></span> (i.e. [Smart brushing](https://youtu.be/VU117h6wT6w?t=576))

::: notes

by design, using criteria present in the data.

by the user, requires interaction / UX design

innovation in the part of how the user interacts with the data

:::

### {data-transition="fade" data-background-iframe="https://www.youtube.com/embed/VU117h6wT6w?controls=0&amp;start=576"}

::: notes

Instead of selecting by line, allows the user to select by pattern

:::

### <span class="pretitle">1. Data visualisation as an artefact</span> The atomic level  {data-transition="fade"}

**2. Split data into multiple charts** <span class="trend"></span>

. . .

Facets, trellis, small multiples.

![Example of small multiples: The Trilogy Meter (Meth 2009)](img/smallmultiples2.jpg){height="300"}

::: notes

Small multiples are sets of charts of the same type, with the same scale, presented together at a small size and with minimal detail, usually in a grid of some kind. The term was at least popularized by Edward Tufte, appearing first in his Visual Display of Quantitative Information in 1983. He says of them:

Small multiples are economical: once viewers understand the design of one [chart], they have immediate access to the data in all the other [charts]… as the eye moves from one [chart to the next, the consistency of the design allows viewers to focus on changes in the data rather than on changes in graphical design.

:::


### <span class="pretitle">1. Data visualisation as an artefact</span> The atomic level  {data-transition="fade"}

**3. Augmenting visualisations** <span class="trend"></span>

. . .

![[ggExtra](https://daattali.com/shiny/ggExtra-ggMarginal-demo/), adding marginal histograms to ggplot2 (by Dean Attali)](img/ggplot-extra.png){height="350"}

::: notes

adding redundant views on the same data

:::

### <span class="pretitle">1. Data visualisation as an artefact</span> The atomic level  {data-transition="fade"}

**4. Densify**

>- Escaping overplotting in scatterplots <span class="trend"></span>

. . .

![Clearly overplotted scatterplot (Kovalyshyn 2017)](img/scatterplot1.png){height="325"}

### <span class="pretitle">1. Data visualisation as an artefact</span> The atomic level  {data-transition="fade"}

**4. Densify**

- Escaping overplotting in scatterplots <span class="trend"></span>

![Using transparency is not helpful (Kovalyshyn 2017)](img/scatterplot2.png){height="325"}

### <span class="pretitle">1. Data visualisation as an artefact</span> The atomic level  {data-transition="fade"}

**4. Densify**

- Escaping overplotting in scatterplots <span class="trend"></span>

![Now we can **see** density (Kovalyshyn 2017)](img/scatterplot-hexbin.png){height="325"}

::: notes

Actually implies statistical simplification.

color is in logaritmic scale.

:::

### <span class="pretitle">1. Data visualisation as an artefact</span> The atomic level  {data-transition="fade"}

**4. Densify**

- Timelines <span class="innovation"></span>

![DenseLines, a density representation of many time series as a heatmap (Moritz & Fisher 2018)](img/stocks_lines.png){height="300"}

::: notes

a stock market dataset of 3,500 historical New York Stock Exchange closing prices.

:::

### <span class="pretitle">1. Data visualisation as an artefact</span> The atomic level  {data-transition="fade"}

**4. Densify**

- Timelines <span class="innovation"></span>

![DenseLines, a density representation of many time series as a heatmap (Moritz & Fisher 2018)](img/stocks.png){height="300"}

::: notes

Dense clusters of lines are easy to spot in blue, while bright yellow shows areas with few stock price lines. The drop that came with the financial crisis in 2008 is clearly visible. Similarly, we can see two dense bands of stock values around $15 and $25, showing that companies (or customers) tend toward round stock prices.

:::

### <span class="pretitle">1. Data visualisation as an artefact</span> The atomic level  {data-transition="fade"}

Adding the time factor:

- Static visualisations with real data (at the time of loading)
- Real-time/evolving visualisations, static and auto-refreshed 
- Streaming data visualisations showing the flow of data

Require an additional effort for operational intelligence, where immediate decision making could be a requirement.

<span class="source">Source: Aragues 2018</span>

<!-- Gapminder: https://youtu.be/hVimVzgtD6w?t=147

https://medium.com/@urban_institute/4-observations-on-animating-your-data-visualizations-cf987b069c35

Periphery plots: https://vimeo.com/363453522
 -->
::: notes

A static visualisation that uses the data that is available when the visualisation is created. Any new data requires a refresh.

A real-time visualisation that looks like the static one but updates itself constantly.

A streaming data visualisation that shows the flow of data and the impact it has on the statistics.

:::

### <span class="pretitle">1. Data visualisation as an artefact</span> The atomic level  {data-transition="fade"}

How to communicate _nothingness_? (Kirk 2014)

###  {data-transition="fade" data-background-iframe="https://www.youtube.com/embed/JqzAuqNPYVM?start=519"}

::: notes

first question we should ask: what is missing?

:::

### <span class="pretitle">1. Data visualisation as an artefact</span> The atomic level  {data-transition="fade"}

How to communicate _nothingness_?

>- **Null** &nbsp; Absence of measurement
>- **Zero** &nbsp; Absence of amount/magnitude
>- **Blank** &nbsp; Try to use _nothing_ to represent _something_

::: notes

`null` in the age of information overload, data absence is more and more significant. may help in the detection of faulty sensors. If models are built filtering nulls, this insight may be lost.

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

::: notes

glass ceiling

:::

### <span class="pretitle">1. Data visualisation as an artefact</span> The atomic level  {data-transition="fade"}

How to communicate _nothingness_?

- **Null** &nbsp; Absence of measurement
- **Zero** &nbsp; Absence of amount/magnitude
- **Blank** &nbsp; Try to use _nothing_ to represent _something_

>- The design should be **invisible**

###  {data-transition="fade" data-background-iframe="https://www.youtube.com/embed/JqzAuqNPYVM?start=1363"}

::: notes

invisible design

:::

### <span class="pretitle">1. Data visualisation as an artefact</span> The atomic level {data-transition="fade-in slide-out"}

Communicating uncertainty, projections,  
and other non-factual data is challenging.

. . .

![Uncertainty visualisations tested in experiments (Kale _et al._ 2019)](img/hop.gif){height="300"} 

::: notes

margins of error must also be communicated, and they are often mistakenly interpreted as the probability for an event to happen.

:::

### <span class="pretitle">1. Data visualisation as an artefact</span> Number of variables <span class="trend"></span>

![&nbsp;](img/munzner-5.2.png){width="400"}

![Visual marks and channels (Munzner 2014)](img/munzner-5.3.png){width="400" style="margin-top:-25px;"}

::: notes

One and only one attribute/variable should be used per channel.

Multiple channels per attribute are possible (redundant encoding),

:::

### <span class="pretitle">1. Data visualisation as an artefact</span> Number of variables <span class="trend"></span>

<br />

It is required to reduce dimensionality (statistically): PCA, factors, clustering.

::: notes

gaphic variables than can be used are limited, a reduction is required. MUMA

:::

### <span class="pretitle">1. Data visualisation as an artefact</span> Generating new idioms <span class="innovation"></span> {data-transition="slide-in fade-out"}

<br />

A word of caution:

- will need to be custom coded
- readers will require training
- correct interpretation may be more time demanding

. . . 

[Xenographics](https://www.xeno.graphics/): Weird <span class="fragment">but (sometimes) useful </span>charts

### <span class="pretitle">1. Data visualisation as an artefact</span> Generating new idioms <span class="innovation"></span> {data-transition="fade"}

<br />

![Horizon charts (Heer 2009)](img/horizonchart.png)

### <span class="pretitle">1. Data visualisation as an artefact</span> Generating new idioms <span class="innovation"></span> {data-transition="fade"}

![Choropleth maps with `tricolore` (Schöley 2018)](img/tricolore.png){height="325"
}

### <span class="pretitle">1. Data visualisation as an artefact</span> Generating new idioms <span class="innovation"></span> {data-transition="fade"}

![Flame graphs (Gregg 2016)](img/flamegraph.svg){height="325"}

### <span class="pretitle">1. Data visualisation as an artefact</span> Multiple Linked Views (MLV) <span class="trend"></span> <span class="innovation"></span> {data-transition="slide-in fade-out"}

>In a MLV system, a dataset is shown in multiple simple visualizations, with the data items shown in the different charts corresponding to each other. The charts in each visualization can be used to highlight, control, or filter the data items shown in the others. 

<span class="source">(Meyer & Fihser 2018)</span>

::: notes

When idioms are not enough to communicate a complex message, combinations of idioms, more complex paragraphs, are required.

:::


### {data-background-iframe="https://www.youtube.com/embed/kiXMn2VPZek" data-transition="fade-in slide-out"}

<span class="source" style="margin-top:600px;">(Lagner, Kister & Dachselt 2019)</span>

::: notes

multiple views, with an innovative UI. Different levels of viewing: overview vs detail.

AND linked views; a selection in one part drives change in another

:::

### <span class="pretitle">1. Data visualisation as an artefact</span> Beyond 2 dimensions <span class="innovation"></span> {data-transition="slide-in fade-out"}

<div class="center" style="padding-top:2em;">
virtual / augmented reality
</div>

### {data-background-iframe="https://www.youtube.com/embed/8j9r9JKIqww" data-transition="fade"}

::: notes

Realidad virtual: Still purely graphic, tú te metes en el gráfico.
:::

### {data-background-iframe="https://www.youtube.com/embed/p4fB_OfoaZA" data-transition="fade"}

::: notes

Realidad aumentada: El gráfico se saca a la realidad y se coordina con elementos de la realidad física.

:::

### <span class="pretitle">1. Data visualisation as an artefact</span> Other senses <span class="innovation"></span> {data-transition="fade"}

![Sonification example and [demo](https://inclusive.interactivethings.io/#/histogram/sonification) (Guillemot 2018)](img/sound.jpg){height="400"}

::: notes

Not exactly visualisation

Sound: improves accesibility. Keyboard navigation enables sound cues for each representation, and the whole chart can be _sonified_.

:::

### <span class="pretitle">1. Data visualisation as an artefact</span> Other senses <span class="innovation"></span> {data-transition="fade-in slide-out"}

![_Smell necklace_ designed to be used with an immersive VR display ([via Twitter](https://twitter.com/NElmqvist/status/1055370456528773120))](img/smell-necklace.png){height="400"}

# 2. Data visualisation as <br />a communication product {data-transition="slide-in fade-out"}

### {data-transition="fade"}

<h2 style="margin-bottom:2em;">2.&nbsp;Data visualisation as a communication product</h2>

>The modern approach to data visualisation is focused on quickly making data visualisation. 

<span class="source">(Meeks 2018)</span>

::: notes

Profile Meeks, Senior Data Visualisation xxxxxx at Netflix.

Even if this section shows the most communicative-social science view, he is actually an engineer.

:::
### {data-transition="fade"}

<h2>2.&nbsp;Data visualisation as a communication product</h2>

Focus on speed affects:

- how data visualisation products are designed
- what tools are used to create them
- the role of the creator in relation to the product
- how engagement with readers in envisioned

::: notes

>This breackneck pace is a real data visualisation constraint.

The fast mode of dataviz is real and important, but when we let it become our only view into what dataviz is, we limit ourselves in planning for how to build, support and design dataviz.

:::

### {data-transition="fade-in slide-out"}

<h2 style="margin-bottom:1em;">2.&nbsp;Data visualisation as a communication product</h2>

>Ultimately, data visualisation is not a technical problem, it's a design problem and, more than that, <span class="highlighted">a communication problem</span>.

<span class="source">(Meeks 2018)</span>

. . .

Let's look at what charts <span class="fragment">**say**</span><span class="fragment">, **mean**</span><span class="fragment">, and **do**.</span>

::: notes

Let's go slow down a bit

:::


### <span class="pretitle">2. Data visualisation as a communication product</span> What charts say {data-transition="slide-in fade-out"}

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

### <span class="pretitle">2. Data visualisation as a communication product</span> What charts say {data-transition="fade"}

**Implicitly**

No chart is an unbiased view of the data, as data visualisation is a manufactured artefact.

<blockquote style="font-size:.8em">
    
    All data is transformed to be in a chart, and the inaction of not designing that transformation carries just as strong an implication as the action of transforming it.

</blockquote>

<span class="source">(Meeks 2018)</span>

::: notes

there is manufacture = subjectivity from the first moment of the data coding/gathering: choice of variables, variable names, gathering means...

:::

### <span class="pretitle">2. Data visualisation as a communication product</span> What charts say {data-transition="fade"}

<table style="margin-top:-25px;">
    <tr>
        <td>
        ![Most _default_ representation of an histogram](img/iraq-redesigned.png){height="450"}
        </td>
        <td class="fragment" data-fragment-index="1">![Original infographic by Simon Scarr (Meeks 2018)](img/iraq.png){height="450"}</td>
    </tr>
</table>

<figure class="fragment" data-fragment-index="1"><figcaption>
Original infographic (right) by Simon Scarr and redesigned, more default representation of an histogram (left), redesigned by Andy Cotgreave (Meeks 2018)</figcaption></figure>

::: notes

Very strong message. Red, bars point down, looks like blood. Very evocative, emphasized by the title.

Rotation: There's still a peak, but the decline is more apparent

Title: To match the main takeaway of the graph

Color: not like blood anymore

"Situation in Iraq is improving" --> Completely different message!

Neither of those charts is lying. The opinionated nature of charts should be acknowledged and embraced. 

:::

### <span class="pretitle">2. Data visualisation as a communication product</span> What charts say {data-transition="fade"}

**Implicitly**

The implicit channel of a data visualisation (the title and other framing elements) can be even more powerful than the explicit channel.

. . .

**How to improve:** Style should be intentional, purposeful and thematically appropriate, not the result of defaults or superficial decisions.

### <span class="pretitle">2. Data visualisation as a communication product</span> What charts say {data-transition="fade"}

**Systematically** 

<br />

>[...] all charts display data and all data is a proxy for the systems that created and measured that data.

<span class="source">(Meeks 2018)</span>

. . .

**How to improve:** Caution not to reveal an underlying system that is proprietary or confidential.

::: notes

There's sort of a cruel irony to the way we simultaneously share these data products so enthusisastically while bemoaning the privacy issues that are necessary for their creation.

:::

### <span class="pretitle">2. Data visualisation as a communication product</span> What charts say {data-transition="fade"}

**Descriptively**

>- internally: axes, labels, annotations
>- externally: surrounding text, figure descriptions, discussions

. . .

Unlike the implicit channel, the descriptive channel is active and purposeful (not subconscious).

. . .

**How to improve:** Consider annotations, labels, axis elements as part of the data visualisation.

### <span class="pretitle">2. Data visualisation as a communication product</span> What charts say {data-transition="fade-in slide-out"}

>By being more explicit in our own understanding of what charts say and how we can systematically describe what they say, we can grow more capable of using the channels available in that expression to our advantage.

<span class="source">(Meeks 2018)</span>

. . .

<div class="center" style="padding-top:.5em;">
What does your chart say that you didn't intend?
</div>
### <span class="pretitle">2. Data visualisation as a communication product</span> What charts mean {data-transition="slide-in fade-out"}

**Intentionally**

<br />

>The mode and purpose of a chart should be well understood by the chart maker and immediately apparent to the chart reader.

<span class="source">(Meeks 2018)</span>

::: notes

Charts mean more than just what they say.

:::

### <span class="pretitle">2. Data visualisation as a communication product</span> What charts mean {data-transition="fade"}

**Historically**

<br />

Charts are products of their time. 

It is important to provide background about the data sources, to enable checking whether they are still based on relevant priorities, dimensions and metrics.

### <span class="pretitle">2. Data visualisation as a communication product</span> What charts mean {data-transition="fade"}

**Historically**

![A Minnesota Department of Health chart on changing obesity rates that relies on BMI will still be around long after we develop a more sophisticated measure of health and yet nowhere on this chart does “BMI” appear (Meeks 2018)](img/obesity.png)

### <span class="pretitle">2. Data visualisation as a communication product</span> What charts mean {data-transition="fade"}

**Culturally**

<br />

Charts should be adapted to the culture they will be consumed in (think user-centered design techniques).

### <span class="pretitle">2. Data visualisation as a communication product</span> What charts mean {data-transition="fade"}

**Contextually**

<br />

Enable removing and adjusting data visualisation elements to reduce complexity, not based on screen size as in responsive data visualisation, but on priority.

### <span class="pretitle">2. Data visualisation as a communication product</span> What charts mean {data-transition="fade-in slide-out"}

<br />

>Meaning-making may sound too soft to the kind of technical professionals that make and read data visualisation but communication without meaning is just noise.

<span class="source">(Meeks 2018)</span>

### <span class="pretitle">2. Data visualisation as a communication product</span> What charts do {data-transition="slide-in fade-out"}


<br />

The most important thing about a chart is its impact. 

### <span class="pretitle">2. Data visualisation as a communication product</span> What charts do {data-transition="fade"}

**Provide insights**

Identify and emphasize the insights that the readers might expect.

. . .

![A simple line chart (left) and the features of that line chart (right)<br /> which may be considered insights by an audience (Meeks 2018)](img/charts-do.png){height="200"}

::: notes

In this example those consist of the maxima/minima of the data (whether as an extent or as individual features), volume of the total data represented, points of interest, volatility of change or overall trend in the direction of change.

:::

### <span class="pretitle">2. Data visualisation as a communication product</span> What charts do {data-transition="fade"}

**Cause change**

<br />

As difficult to measure as it is important.

How have they impacted business decisions? How were they used in presentations? Where they modified (changed colours, cropped, annotated) somehow?

::: notes

Understanding how a particular chart was an effective piece of evidence or motivation is key to developing more effective data visualisation.

:::

### <span class="pretitle">2. Data visualisation as a communication product</span> What charts do {data-transition="fade"}

**Cause visual literacy**

<br />

>All data visualisation was, at some point, complex data visualisation, until an audience grew comfortable and literate enough to read it.

<span class="source">(Meeks 2018)</span>

::: notes

Languages are live things, that evolve over time, and require breakthrough.

>[...] the new form cannot be introduced until it is understood but can only be understood once it's introduced.

:::

### <span class="pretitle">2. Data visualisation as a communication product</span> What charts do {data-transition="fade"}

**Cause visual literacy**

![This example of a connected scatterplot, used in production at Netflix, has built into it a link to an animated explanation of how to read the new chart along with more familiar charts around it to reduce friction (Meeks 2018)](img/connected-scatterplot.png){height="325"}


### <span class="pretitle">2. Data visualisation as a communication product</span> What charts do {data-transition="fade"}

**Create new charts**

![Imaginary genealogy for charts with scatterplots as a common ancestor (Meeks 2018)](img/genealogy.png){height="350"}

::: notes

Catalogs of data visualisation have the tendency to treat every form as a category of one without drawing connections between them, which disguises how charts lead to other charts.

chart lineage

:::

### <span class="pretitle">2. Data visualisation as a communication product</span> What charts do {data-transition="fade-in slide-out"}

<br />

>All communication is evaluated based on content, but persuasive communication, which is all data visualisation unless it is purely decorative, is rightly also evaluated based on effect.

<span class="source">(Meeks 2018)</span>

::: notes

persuasive in the sense of driving decision or actions on users.

Ultimately, what charts do may be the one most important thing.

:::

# 3. The artefact<br />goes social

### <span class="pretitle">3. The artefact goes social</span> Data counseling {data-transition="slide-in fade-out"}

<br />

>[...] brings domain expertise into the operationalization process to help inform decisions about good proxies as well as to uncover insights using the resulting visualisations.

<span class="source">(Meyer & Fisher 2018)</span>

::: notes

proxies = the best indicator to answer to the questions that you have.

:::

### <span class="pretitle">3. The artefact goes social</span> Data counseling {data-transition="fade"}

Based on **interviews** (1) for

>- gaining an understanding of the questions and data
>- get feedback on proxies, explorations, and visualisation **prototypes** (2)

### <span class="pretitle">3. The artefact goes social</span> Data counseling {data-transition="fade"}

**Interviews**

>The role of the interviewer is to ask questions that will guide the stakeholders toward elucidating the information necessary for working through an operationalization process and designing visualisations.

<span class="source">(Meyer & Fisher 2018)</span>

### <span class="pretitle">3. The artefact goes social</span> Data counseling {data-transition="fade"}

**Interviews**

Identify stakeholders:

>- analysts
>- data producers
>- gatekeepers
>- decision makers
>- connectors

### <span class="pretitle">3. The artefact goes social</span> Data counseling {data-transition="fade"}

**Interviews**

Require practice and experience.

Semistructured: be prepared, but also be open.

>- start with open ended questions (problem, data, context)
>- use the conversation to search out the more abstract question

::: notes

unstructured: can uncover unknown needs and goals, but it can take a significant amount of time to get to anything useful.

structured: while efficient, leave little room for discovering new insights.

:::

### <span class="pretitle">3. The artefact goes social</span> Data counseling {data-transition="fade"}

**Interviews**

Use traditional conversation / interpersonal communication skills to prevent dead ends: keep them talking

>- rephrase responses back to the stakeholder
>- ask the same or similar questions in different ways
>- explore a completely different conversational topic

### <span class="pretitle">3. The artefact goes social</span> Data counseling {data-transition="fade"}

**Interviews**

Contextual interviews

>- take place in the stakeholder's work environment
>- consist of demonstrations of the tools and data inspection methods currently in use

::: notes

often starts by asking the stakeholder to either walk through a specific analysis task they have already performed or conduct someof their work for that day with the interviewer present. The stakeholder talks through each step they are taking.

:::

### <span class="pretitle">3. The artefact goes social</span> Data counseling {data-transition="fade"}

**Rapid prototyping**

<br />

>[...] is a process of trying out many visualisation ideas as quickly as possible and getting feedback from stakeholders on their efficacy.

<span class="source">(Meyer & Fisher 2018)</span>

### <span class="pretitle">3. The artefact goes social</span> Data counseling {data-transition="fade"}

**Rapid prototyping**

<br />

<div class="center">

&ne; _fast_ data visualisation

</div>

. . .

<div class="center">

&ap; agile/lean methodologies  
and user-centered design

</div>

::: notes

NOT to be confused with **fast** dataviz

:::

### <span class="pretitle">3. The artefact goes social</span> Data counseling {data-transition="fade"}

**Rapid prototyping**

<br />

![Prototypes range from low-fidelity sketches to high-fidelity working models (Meyer & Fisher 2018)](img/prototypes.png)

::: notes

low-fi: sketched on paper or on a whiteboard, digital mockups that may include some controls for explaining interaction ideas (slides). Can incorporate charts generated in Excel or Tableau with fake or sampled data. Great for communicatingthe gist of an idea in an interview, fast and easy to produce. Rapidly establish whether the visualisationd designer is on the same page as the stakeholders.

hi-fi: custom visualisations which must be created from scratch. Largely contain the core functionality. Meant to be thrown away, the point is not to worry about the code other than to confirm that ideas can work.

:::

### <span class="pretitle">3. The artefact goes social</span> Data counseling {data-transition="fade"}

**Rapid prototyping**

Prototypes are made to obtain feedback on them: get to the stakeholders early and often.

Focus not on whether they like it or not, but rather on **what the visualisation can and cannot do** (contextual interview where the stakeholder uses the visualisation).

### <span class="pretitle">3. The artefact goes social</span> Responsive data visualisation {data-transition="fade"}

<br />

>Responsive web design, and responsive data visualisation are not simply a way to make our content accessible on smaller screens. We need to build an ergonomic web that feels natural regardless of device type.

<span class="source">(Hinderman 2018)</span>

### <span class="pretitle">3. The artefact goes social</span> Responsive data visualisation {data-transition="fade"}

<br />

Unknowns require adaptability.

>- the context in which **the user** is trying to consume the visualisation
>- changes in **the data** that is being displayed

::: notes

the user: core of responsive web design as a whole

the data: unique to data visualisation. This is what makes a visualisation FULLY responsive _vs._ simply scaling them at different viewport sizes, like an image.

>[...] every single thing that you can do to make your visualisation more clear, more usable, or more communicative is a reaction to either the context in which the user is trying to consume it, or a change in the data being displayed.

:::

### <span class="pretitle">3. The artefact goes social</span> Responsive data visualisation {data-transition="fade"}

**Output side (the client)**

Making things work in all screen types by redrawing charts to fit its container. 

Match CSS breakpoints + add any new ones as the content requires: group data to fit (trade-off precision for reduced rendering complexity and performance).

::: notes

With a combination of CSS and D3.

Breakpoints: build for your smallest supported screen: then, as you find a spot at which it makes sense to redraw, create a new breakpoint there.

:::

### <span class="pretitle">3. The artefact goes social</span> Responsive data visualisation {data-transition="fade"}

**Input side (the data)**

Adapting at breakpoints. No need to just redraw the exact same elements:

>As long as the message being conveyed by the data is the same, and the point you're trying to prove is always present, you should prove it with as much firepower as you have available.

<span class="source">(Hinderman 2018, p.361)</span>

::: notes

We need to KNOW 

- what is the message being conveyed by the data (what does it SAY)
- what is the point you're trying to prove (what does it MEAN)

:::

### <span class="pretitle">3. The artefact goes social</span> Responsive data visualisation {data-transition="fade"}

**Input side (the data)**

Adapting at interaction points. 

>[...] present a rational default but enable users to dig into more complex or specific layers of data when the device's capabilities limit the presentation of both at the same time.

<span class="source">(Hinderman 2018, p.362)</span>

::: notes

The most crucial and digestive information should be prioritised, but interaction should enable more granularity.

:::

### <span class="pretitle">3. The artefact goes social</span> Responsive data visualisation {data-transition="fade"}

Different views on heartreate depending on device:

<br />

![Garmin watch](img/garmin-watch.jpg){width="200"} 

### <span class="pretitle">3. The artefact goes social</span> Responsive data visualisation {data-transition="fade"}

Different views on heartreate depending on device:

![Garmin Android app, portrait and landscape views](img/garmin-mobile.png){height="350"}

### <span class="pretitle">3. The artefact goes social</span> Responsive data visualisation {data-transition="fade"}

Different views on heartreate depending on device:

<br />

![Garmin website from desktop](img/garmin-desktop.gif)



### <span class="pretitle">3. The artefact goes social</span> Responsive data visualisation {data-transition="fade"}

![Linear and radial temperature range charts designed for mobile phone displays (Brehmer _et al._ 2019)](img/temperature-mobile.png){height="350"}

::: notes

In adapting to different devices, perception of different kinds of charts may differ. 

:::

### {data-background-iframe="https://www.youtube.com/embed/MwJmjTBfOx0" data-transition="fade-in slide-out"}

::: notes

a vast majority of smartwatch interactions last under 5 s. Some chart types are not apropriate for certain devices.

:::

<!--
### <span class="pretitle">3. The artefact goes social</span> Responsive data visualisation {data-transition="fade"}

The other "side" of adaptation is on the side of the user.

Data served

### Responsive data visualisation

Device dependant

### Responsive data visualisation

Alerts

Example: sports tracker on watch vs. phone vs. computer -->

# Epilogue

### 

![(Meeks 2017)](img/data-matrix.jpg){style="margin-top:2em;"}

::: notes

Data visualisation is a communication product. 

There is no such thing as raw data, and there is neither such a thing as a raw data visualization (aseptic, unbiased view on the data). Even if we understood datavis as a photograph of the data, photos are long taken as political products, with a meaning, and one view of reality and not another one. But what's more, I wouldn't even say that datavis are photos of the data, they are more illustrations, drawings of the data, more crafted than photographs. And as such, we should draw them with purpose, and we should draw them FOR the user/the reader, meaning we should make them adapted, and responsive.

:::

---

<h1>Thank you!</h1>

<div class="center">

This presentation is available at  
[`https://mrn.bz/BDAP2018`](https://mrn.bz/BDAP2018)

</div>

<div  class="center" style="font-family:Roboto, sans-serif;font-size:.5em;padding-top:2em; margin:0 auto;" markdown="1">

<hr style="margin-top:2em; border-color:#999; border-top:none;" />

![](img/deustokomunika-logo.png){width="50" style="vertical-align:middle;"}
[&#64; DeustoKomunika](http://twitter.com/deustokomunika)  ![](img/deustodatacom-logo.png){width="50" style="vertical-align:middle;padding-left:25px;"}
[&#64; DeustoData](http://twitter.com/deustodata) [&#64; mberasategi](http://twitter.com/mberasategi){style="padding-left:25px;"} [&#64; neregauzak](https://twitter.com/neregauzak){style="padding-left:25px;"}

</div>


### Resources

<div style="font-size:.7em !important;">

- [D3.js](https://d3js.org/)    
    A JavaScript library for manipulating documents based on data. D3 helps you bring data to life using HTML, SVG, and CSS.
- [ggplot2](https://ggplot2.tidyverse.org/)  
    Data visualization package for the statistical programming language R. 
- [IEEEVIS 2019](http://ieeevis.org/year/2019/info/papers-sessions)  
    Conference on Scientific Visualisation, Information Visualisation and Visual Analytics. Papers from the 2018 edition.
- [matplotlib](https://matplotlib.org/), [seaborn](https://seaborn.pydata.org/)  
    Just two of the many data visualisation libraries available for Python
- [Open Access Vis](http://oavis.steveharoz.com/)  
   A collection of open access visualisation research at the VIS 2018 conference.
- [Xenographics](http://xeno.graphics)  
   Weird but (sometimes) useful charts.
- [Data Visualisation Catalogue](https://datavizcatalogue.com/index.html)
   A library of different information visualisation types.

</div>

### References

<div class="source refs">

<div style="width:48%;float:left;">

Anthony Aragues (2018), _Visualizing Streaming Data_. O'Reilly Media

Tanja Blascheck, Lonni Besançon, Anastasia Bezerianos, Bongshin Lee, Petra Isenberg (2019). "[Glanceable Visualization: Studies of Data Comparison Performance on Smartwatches](https://www.microsoft.com/en-us/research/publication/glanceable-visualization-studies-of-data-comparison-performance-on-smartwatches/)". _IEEE Transactions on Visualization and Computer Graphics_ 25(1) [`10.1109/TVCG.2018.2865142`](https://ieeexplore.ieee.org/document/8443125)`

Matthew Brehmer, Bongshin Lee, Petra Isenberg, Eun Kyoung Choe (2019). "[Visualizing Ranges over Time on Mobile Phones: A Task-Based Crowdsourced Evaluation](https://www.microsoft.com/en-us/research/publication/visualizing-ranges-over-time-on-mobile-phones-a-task-based-crowdsourced-evaluation/)". _IEEE Transactions on Visualization and Computer Graphics_ 25(1) [`10.1109/TVCG.2018.2865234`](https://ieeexplore.ieee.org/document/8440812)

Brendan Gregg (2016), "[The Flame Graph](https://queue.acm.org/detail.cfm?id=2927301)". _ACM Queue_ 14(2)

Luc Guillemot (2018), "[How Does This Data Sound?](https://blog.interactivethings.com/how-does-this-data-sound-945ed27a1a95)"

Jeffrey Heer, Nicholas Kong, Maneesh Agrawala (2009), "[Sizing the Horizon: The Effects of Chart Size and Layering on the Graphical Perception of Time Series Visualizations](http://vis.berkeley.edu/papers/horizon/)". _ACM Human Factors in Computing Systems (CHI)_, pp. 1303 - 1312 [`10.1145/1518701.1518897`](https://dl.acm.org/citation.cfm?doid=1518701.1518897)

Bill Hinderman (2015), _Building Responsive Data Visualization for the Web_. O'Reilly

Christophe Hurter, Nathalie Henry Riche, Steven M. Drucker, Maxime Cordeil, Richard Alligier, Romain Vuillemot (2018), "[FiberClay: Sculpting Three Dimensional Trajectories to Reveal Structural Insights](http://recherche.enac.fr/~hurter/FiberClay.html)", _IEEE Transactions on Visualization and Computer Graphics_ 25(1)

Alex Kale, Francis Nguyen, Matthew Kay, Jessica Hullman (2019), "[Hypothetical Outcome Plots Help Untrained Observers Judge Trends in Ambiguous Data](https://idl.cs.washington.edu/papers/hops-trends/)", _IEEE Transactions on Visualization and Computer Graphics_ 25(1) 

</div>

<div style="width:48%;float:right;">

Andy Kirk (2014), "[The Design of Nothing: Null, Zero, Blank](https://www.youtube.com/watch?v=JqzAuqNPYVM)", _OpenVis Conference 2014_

Ihor Kovalyshyn (2017), ["When Scatter Plot Doesn't Work"](https://delta1epsilon.github.io/2017/When-Scatter-Plot-doesn%27t-work/)

Ricardo Langner, Ulrike Kister, Raimund Dachselt (2019). "[Multiple Coordinated Views at Large Displays for Multiple Users: Empirical Findings on User Behavior, Movements, and Distances](https://imld.de/en/research/research-projects/mcv-displaywall/)", _IEEE Transactions on Visualization and Computer Graphics_ 25(1)  (proc. InfoVis 2018) [`10.1109/TVCG.2018.2865235`](https://doi.org/10.1109/TVCG.2018.2865235)

Elijah Meeks (2017), ["Strategic Innovation in Data Visualization Will Not Come From Tech"](https://medium.com/visualizing-the-field/strategic-innovation-in-data-visualization-will-not-come-from-tech-4c1f7379ae39)

&mdash; (2018), "[Data Visualization, Fast and Slow](https://medium.com/@Elijah_Meeks/data-visualization-fast-and-slow-d2653d4850b0)"

Dan Meth (2009), "[The Trilogy Meter](https://danmeth.myportfolio.com/post/77471620/my-trilogy-meter-1-in-a-series-of-pop-cultural)" 

Miriah Meyer & Danyel Fisher (2018), _Making Data Visual_. O'Reilly Media

Dominik Moritz and Danyel Fisher (2018), "Visualizing a Million Time Serieswith the Density Line Chart" [ arXiv:1808.06019v2](https://arxiv.org/pdf/1808.06019.pdf) [cs.HC]

Tamara Munzner (2015). _Visualization Analysis and Design_. CRC Press

Jonas Schöley (2018), "[Choropleth maps with tricolore](https://cran.r-project.org/web/packages/tricolore/vignettes/choropleth_maps_with_tricolore.html)"

Ronell Sicat, Jiabao Li. [_DXR: A Toolkit for Building Immersive Data Visualizations_](https://sites.google.com/view/dxr-vis/download?authuser=0)

</div>


--- 

<h1>License</h1>

<div style="text-align:center;margin-top:3.5em;">

![](img/cc/cc.logo.png){height="50px" style="display:inline-block;margin-right:2em;"}
![](img/cc/by.png){height="50px" style="display:inline-block;"}
![](img/cc/sa.png){height="50px" style="display:inline-block;"}

</div>

<p style="font-family:Roboto, Montserrat, Helvetica, Arial, sans-serif; font-size:.3em;font-weight:200;margin-top:3em;">Copyright &copy; 2018 University of Deusto<br />
This work (except for the quoted images, whose rights are reserved to their owners) is licensed under the Creative Commons “Attribution-ShareAlike” License. To view a copy of this license, visit [http://creativecommons.org/licenses/by-sa/3.0/](http://creativecommons.org/licenses/by-sa/3.0/)</p>