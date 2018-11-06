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

### Graphic constraints  {data-transition="slide-in fade-out"}

> 1. Number of observations / marks

. . .

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

### Graphic constraints  {data-transition="slide-in fade-out"}

1. Number of observations / marks

. . .

Some strategies to overcome these constraints:

>1. Filter
>2. Facets/small multiples
>3. Augmenting visualizations
>4. Densify

### {data-transition="fade"}

**1. Filter observations**

>- By design <span class="trend"></span>
>- By allowing the user to filter according to their interests <span class="trend"></span>
>    + Innovative filtering <span class="innovation"></span> (i.e. [Smart brushing](https://youtu.be/VU117h6wT6w?t=576))

### {data-transition="fade" data-background-iframe="https://www.youtube.com/embed/VU117h6wT6w?controls=0&amp;start=576"}

### {data-transition="fade"}

**2. Facets/small multiples** <span class="trend"></span>

Hemen zerbait? erreferentziaren bat?

### {data-transition="fade"}

**3. Augmenting visualizations** <span class="trend"></span>

. . .

![[ggExtra](https://daattali.com/shiny/ggExtra-ggMarginal-demo/), adding marginal histograms to ggplot2 (by Dean Attali)](ggplot-extra.png)

### {data-transition="fade"}

**4. Densify**

>- Escaping overplotting in scatterplots <span class="trend"></span>

. . .

![Clearly overplotted scatterplot](scatterplot1.png){height="325"}

<span class="source">Source: Ihor Kovalyshyn (2017), [_When Scatter Plot Doesn't Work_](https://delta1epsilon.github.io/2017/When-Scatter-Plot-doesn%27t-work/)</span>

### {data-transition="fade"}

**4. Densify**

- Escaping overplotting in scatterplots <span class="trend"></span>

![Using transparency is not helpful](scatterplot2.png){height="325"}

<span class="source">Source: Ihor Kovalyshyn (2017), [_When Scatter Plot Doesn't Work_](https://delta1epsilon.github.io/2017/When-Scatter-Plot-doesn%27t-work/)</span>

### {data-transition="fade"}

**4. Densify**

- Escaping overplotting in scatterplots <span class="trend"></span>

![Now we can **see** density](scatterplot-hexbin.png){height="325"}

<span class="source">Source: Ihor Kovalyshyn (2017), [_When Scatter Plot Doesn't Work_](https://delta1epsilon.github.io/2017/When-Scatter-Plot-doesn%27t-work/)</span>


### {data-transition="fade"}

**4. Densify**

- Timelines <span class="innovation"></span>

![DenseLines, a density representation of many time series as a heatmap](denselines.png){height="325"}

<span class="source">Source: Dominik Moritz and Danyel Fisher (2018), "Visualizing<br />  a Million Time Serieswith the Density Line Chart" [ arXiv:1808.06019v2](https://arxiv.org/pdf/1808.06019.pdf) [cs.HC]</span>


### Graphic constraints  {data-transition="fade"}

1. Number of observations / marks

About real time... ?¿

### Graphic constraints  {data-transition="fade"}

1. Number of observations / marks

Non-existing data

... elaborate

###  {data-transition="fade" data-background-iframe="https://www.youtube.com/embed/JqzAuqNPYVM"}

### Graphic constraints  {data-transition="fade-in slide-out"}

1. Number of observations / marks

Projections, statistical models, uncertainty

Unpublished papers:

<span class="source left">Alex Kale, Francis Nguyen, Matthew Kay, Jessica Hullman (2019), "[Hypothetical Outcome Plots Help Untrained Observers Judge Trends in Ambiguous Data](https://idl.cs.washington.edu/papers/hops-trends/)", _IEEE Trans. Visualization & Comp. Graphics (Proc. InfoVis)_, 2019</span>

<span class="source left">Jessica Hullman, Xiaoli Qiao, Michael Correll, Alex Kale, Matthew Kay (2019), "[In Pursuit of Error: A Survey of Uncertainty Visualization Evaluation](https://idl.cs.washington.edu/papers/uncertainty-eval-survey)", _IEEE Trans. Visualization & Comp. Graphics (Proc. InfoVis)_</span>

### Graphic constraints

2. Number of variables

- Reduce dimensionality (statistically)
- Restructure dataset (from wide to tall): PCA, factors, clusters

### Graphic constraints  {data-transition="slide-in fade-out"}

3. Generating a new graphical language <span class="innovation"></span>

A word of caution:

- will need to be custom coded
- readers will require training
- correct interpretation may be more time demanding

### Graphic constraints  {data-transition="fade"}

3. Generating a new graphical language <span class="innovation"></span>

![Horizon charts](horizonchart.png)
  
<span class="source">Source: Jeffrey Heer, Nicholas Kong, Maneesh Agrawala (2009), "[Sizing the Horizon: The Effects of Chart Size and Layering on the Graphical Perception of Time Series Visualizations](http://vis.berkeley.edu/papers/horizon/)". _ACM Human Factors in Computing Systems (CHI)_, pp. 1303 - 1312</span>

### Graphic constraints  {data-transition="fade"}

3. Generating a new graphical language <span class="innovation"></span>

![Choropleth maps with `tricolore`](tricolore.png){height="325"
}
 
<span class="source">Source: Jonas Schöley (2018), "[Choropleth maps with tricolore](https://cran.r-project.org/web/packages/tricolore/vignettes/choropleth_maps_with_tricolore.html)"</span>

### Graphic constraints  {data-transition="fade"}

3. Generating a new graphical language <span class="innovation"></span>

![Flame graphs](flamegraph.svg){height="325"
}
 
<span class="source">Source: Brendan Gregg (2016), "[The Flame Graph](https://queue.acm.org/detail.cfm?id=2927301)". _ACM Queue_ Vol. 14, No. 2</span>

### {data-background-image="flamegraph.svg" data-transition="fade-in slide-out"}

### Multiple Linked Views (MLV) <span class="trend"></span> <span class="innovation"></span> {data-transition="slide-in fade-out"}

_Making Data Visual_

Graph thumbnails?

<span class="source">
Ricardo Langner, Ulrike Kister, Raimund Dachselt (2019). "[Multiple Coordinated Views at Large Displays for Multiple Users: Empirical Findings on User Behavior, Movements, and Distances](https://imld.de/en/research/research-projects/mcv-displaywall/)", _IEEE Transactions on Visualization and Computer Graphics_ 25(1) (InfoVis 2018, Berlin) [`10.1109/TVCG.2018.2865235`](https://doi.org/10.1109/TVCG.2018.2865235)</span>

### {data-background-iframe="https://www.youtube.com/embed/kiXMn2VPZek" data-transition="fade-in slide-out"}

### Virtual Reality <span class="innovation"></span> {data-transition="slide-in fade-out"}

### {data-background-iframe="https://www.youtube.com/embed/p4fB_OfoaZA" data-transition="fade"}

### {data-background-iframe="https://www.youtube.com/embed/8j9r9JKIqww" data-transition="fade"}

### Virtual Reality <span class="innovation"></span> {data-transition="fade-in slide-out"}

References:

<span class="source left">
Ronell Sicat, Jiabao Li. [_DXR: A Toolkit for Building Immersive Data Visualizations_](https://sites.google.com/view/dxr-vis/download?authuser=0)
</span>

<span class="source left">
Christophe Hurter, Nathalie Henry Riche, Steven M. Drucker, Maxime Cordeil, Richard Alligier, Romain Vuillemot (2018), "[FiberClay: Sculpting Three Dimensional Trajectories to Reveal Structural Insights](http://recherche.enac.fr/~hurter/FiberClay.html)", IEEE Transactions on Visualization and Computer Graphics_ 25(1) (InfoVis 2018, Berlin)</span>

### Senses and control interfaces <span class="innovation"></span>

(How is this _visualization_?)

- Wheeled micro robots
- Sound
- _smell necklace_ https://twitter.com/NElmqvist/status/1055370456528773120

## 2. Data visualization as a tool for communication

### What charts say {data-transition="fade"}


### What charts say {data-transition="fade"}

Explicitly

### What charts say {data-transition="fade"}

Implicitly

### What charts say {data-transition="fade"}

Systematically

### What charts say {data-transition="fade-in slide out"}

Descriptively

### What charts mean

### What charts do

## 3. The artifact goes social

### Data counseling

### Responsive data visualization

Data served

### Responsive data visualization

Device dependant

### Responsive data visualization

Alerts
