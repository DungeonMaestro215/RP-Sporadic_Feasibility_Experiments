# Data 

This data is organized by the chosen processor configuration.

## Configurations
  - `identical`: All processors have the same speed of 0.8. Note: 1.0 was not chosen so that some heavier tasks would require parallelism.
  - `identical-random`: All processors have the same speed chosen uniformly from [0.5, 0.9]
  - `random`: Every processor and task pair has a different speed, chosen uniformly from [0.0, 1.0].
  - `uni-three-speed`: Three speed classes for Uniform. Fast = 0.8, Medium = 0.5, Slow = 0.3.
  - `uni-three-speed-random`: Three speed classes for Uniform, chosen randomly. Fast from [0.6, 0.9], Medium from [0.3, 0.5], Slow from [0.1, 0.2].
  - `uni-two-speed`: Two speed classes for Uniform. Fast = 0.8, Slow = 0.4.
  - `uni-two-speed-random`: Two speed classes for Uniform, chosen randomly. Fast from [0.5, 0.9], Slow from [0.1, 0.4].
  - `unr-three-speed-random`: Three speed classes for Unrelated. Every processor and task pair has a different speed. Fast from [0.6, 0.9], Medium from [0.3, 0.5], Slow from [0.1, 0.2].
  - `unr-two-speed-random`: Two speed classes for Unrelated. Every processor and task pair has a different speed. Fast from [0.5, 0.9], Slow from [0.1, 0.4].

## Formatting
Data is stored as a `.csv` file for each choice of utilization distribution, processor speed distribution, and processor count. Each configuration appears in three experiments:
  - `avgPExperiment`: Average Necessary Parallelism to achieve feasibility
  - `feasibilityExperiment` with p = 1: Proportion of generated systems feasible with parallelism levels of 1
  - `feasibilityExperiment` with p = m: Proportion of generated systems feasible with parallelism levels of m

Each file contains the following four columns, in order:
  - Utilization
  - Unrelated
  - Uniform
  - Identical

The first column gives the utilizations of generated task sets. The last three are the results for the Unrelated, Uniform, and Identical system models, respectively.

Some data points are recorded as `nan`. This indicates that not enough of the generated task sets with the corresponding specifications could be made feasible.
