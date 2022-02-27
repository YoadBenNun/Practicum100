# Machine learning, efficiency and gold recovery from ores

## Task Statement
Zyfra is a leading provider of efficient solutions for a variety of industries.
This study aims to develop a model that can predict the amount of gold recovered from gold ores.
The model will help to optimize the production and eliminate unprofitable parameters.



## Description of the data

#### Technological process

- `Rougher feed`      — raw material
- `Rougher additions` — flotation reagents: Xanthate, Sulphate, Depressant (or *reagent additions*)
    - `Xanthate`      — promoter or flotation activator;
    - `Sulphate`      — sodium sulphide for this particular process;
    - `Depressant`    — sodium silicate.
- `Rougher process`   — flotation
- `Rougher tails`     — product residues
- `Float banks`       — flotation unit
- `Cleaner process`   — purification
- `Rougher Au`        — rougher gold concentrate
- `Final Au`          — final gold concentrate

#### Parameters of stages

- `air amount`   — the volume of air
- `fluid levels` — level of fluids
- `feed size`    — feed particle size
- `feed rate`    — feeding rate

#### Feature naming

Here's how the features are named:

`[stage].[parameter_type].[parameter_name]`

Example: `rougher.input.feed_ag`

Possible values for `[stage]`:

- `rougher`           — flotation
- `primary_cleaner`   — primary purification
- `secondary_cleaner` — secondary purification
- `final`             — final characteristics

Possible values for `[parameter_type]`:

- `input`       — raw material parameters
- `output`      — product parameters
- `state`       — parameters characterizing the current state of the stage
- `calculation` — calculation characteristics


## Summary
In this project, we studied data provided by a metal mining company to train a model that would predict the most efficient process to extract gold out of ores.
Based on data collected by IoT sensors along the production line we can estimate the concentrations and amounts of different substances and techniques needed to extract the most gold out of the ores.

### Challenges
There were quite a few challenges in this project regarding data preparation and pre-processing.
- The data provided had a high portion of missing values in different parts of the datasets.
- The data provided had a high dimensionality due to a complex process of production.
- The missing values in our data were quite random, each production is different, with different input, and different processes of extraction. That made filling these values quite a challenge.
- Due to a complex production process, our metric of evaluation had to be custom-made to evaluate the model’s performance.
