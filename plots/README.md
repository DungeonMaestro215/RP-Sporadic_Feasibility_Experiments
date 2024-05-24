# Plots

These plots are organized by the chosen processor configuration.

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
