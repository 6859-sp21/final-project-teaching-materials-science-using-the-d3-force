# Teaching Materials Science using the (d3-)force
##### Georgios Varnavides
An interactive narrative teaching materials science concepts with molecular-dynamics simulations, (ab-)using the d3-force module.

## Project Components
The project consists of two parts
- Development of an extension to d3-force module, called `d3-force-md`, to include:
  - _True_ velocity-verlet integration (force averaging, with finite time-step)
  - **Updated** `forceLink` force to ensure energy-conservation
  - Implementation of two **new** forces, common in molecular dynamics simulations
- Interactive narrative using `d3-force-md` to teach Materials Science concepts
  - Aimed at undergraduate students

## Project Deliverables

### * `d3-force-md` Module

The module source code is hosted in its [own repository](https://github.com/gvarnavi/d3-force-md).
Forked from the [`d3-force` repository](https://github.com/d3/d3-force), the main contributions can be found in the following files: [src/simulation.js](https://github.com/gvarnavi/d3-force-md/blob/master/src/simulation.js), [src/link.js](https://github.com/gvarnavi/d3-force-md/blob/master/src/link.js), [src/lennardJonesPotential.js](https://github.com/gvarnavi/d3-force-md/blob/master/src/lennardJonesPotential.js), [src/centralPotential.js](https://github.com/gvarnavi/d3-force-md/blob/master/src/centralPotential.js).

#### Installation
The module is [published on NPM](https://www.npmjs.com/package/d3-force-md), and can be installed using `npm install d3-force-md`. Alternatively, it can also be used as a [standalone library](https://unpkg.com/d3-force-md). AMD, CommonJS, and vanilla environments are supported. In vanilla, a `d3` global is exported:

```html
<script src="https://d3js.org/d3-dispatch.v2.min.js"></script>
<script src="https://d3js.org/d3-quadtree.v2.min.js"></script>
<script src="https://d3js.org/d3-timer.v2.min.js"></script>
<script src="https://unpkg.com/d3-force-md"></script>
<script>

var simulation = d3.forceSimulation(nodes);

</script>
```
#### Documentation
In addition to the full documentation found in the [module repository](https://github.com/gvarnavi/d3-force-md), a trimmed version highlighting the changes introduced to the API can be found in this [notebook](https://observablehq.com/@gvarnavi/d3-force-md-documentation). A comparison with the `d3-force` module can also be found in this [notebook](https://observablehq.com/@gvarnavi/introduction-to-d3-force-md).

### * Interactive Narrative
The interactive narrative, deployed as an [Observable notebook](https://observablehq.com/@gvarnavi/teaching-materials-science-concepts-using-the-d3-force), uses the `d3-force-md` module to introduce a variety of Materials Science concepts such as:
- Lattice dynamics  

[<img alt="Lattice Dynamics" src="https://raw.githubusercontent.com/6859-sp21/final-project-teaching-materials-science-using-the-d3-force/master/img/lattice-dynamics.png" width="420" height="219">]

- Physical origin of surface energy

[<img alt="Surface Energy" src="https://raw.githubusercontent.com/6859-sp21/final-project-teaching-materials-science-using-the-d3-force/master/img/surface_energy_slide_graphic.png" width="420" height="219">]

- Dislocations during materials deformation

[<img alt="Dislocations" src="https://raw.githubusercontent.com/6859-sp21/final-project-teaching-materials-science-using-the-d3-force/master/img/dislocations.png" width="420" height="219">]

- An interactive simulation playground

[<img alt="Playground" src="https://raw.githubusercontent.com/6859-sp21/final-project-teaching-materials-science-using-the-d3-force/master/img/playground.png" width="420" height="219">]

### * Project Video
The 1-minute video teaser can be found [here](https://www.youtube.com/watch?v=LzqRPEFKq3o).

### * Project Paper
The paper describing the project in more detail can be found [here](https://github.com/6859-sp21/final-project-teaching-materials-science-using-the-d3-force/blob/master/FinalPaper.pdf).

## Project Process and Acknowledgments
```diff
!TO-DO
```
