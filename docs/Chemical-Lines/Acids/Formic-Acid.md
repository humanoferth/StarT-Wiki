# Formic Acid

Formic acid is an acid available as early as <LV>**LV**</LV>. While it is not used in any major recipes, it is notable for its use in the formic acid loop, which takes in water and outputs hydrogen and oxygen.

## How to make Formic Acid

Formic acid is made from carbon dioxide (from liquid air distillation) and water.

![Formic recipe](docs/Chemical-Lines/Acids/CH2O2_img/chemical_reactor_formic_acid.png)

## How to make the Formic Acid Loop

```mermaid
flowchart LR;
    %%{init: { 'theme': 'neutral', 'themeVariables': { 'edgeLabelBackground': 'transparent', 'secondaryColor': 'transparent', 'tertiaryColor': 'transparent', 'labelBkgBackground' : 'transparent' }}}%%

    A@{ img: "https://start-dev-team.github.io/StarT-Wiki/Chemical-Lines/Acids/CH2O2_img/chemical_reactor_carbon_dioxide_from_carbon.png", label: "Chemical Reactor", pos: "t", w: 200, h: 200, constraint: "on" }

    B@{ img: "https://start-dev-team.github.io/StarT-Wiki/Chemical-Lines/Acids/CH2O2_img/chemical_reactor_formic_acid.png", label: "Chemical Reactor", pos: "t", w: 200, h: 200, constraint: "on" }

    C@{ img: "https://start-dev-team.github.io/StarT-Wiki/Chemical-Lines/Acids/CH2O2_img/electrolyzer_decomposition_electrolyzing_formic_acid.png", label: "Chemical Reactor", pos: "t", w: 200, h: 200, constraint: "on" }

    D@{ shape: lean-r, label: "1b Water" }

    E@{ shape: lean-r, label: "1b Oxygen" }

    F@{ shape: lean-r, label: "2b Hydrogen" }

    A --1b Carbon Dioxide--> B --1b Formic Acid--> C;

    D --> B
    B --> E
    C --> F
```