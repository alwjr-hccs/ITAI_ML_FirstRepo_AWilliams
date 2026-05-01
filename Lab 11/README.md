What is the main difference between a model parameter and a hyperparameter? Model parameters are learned from the data during training. Examples: decision tree splits, neural network weights, logistic regression coefficients.
Hyperparameters are set before training and control how the model learns. Examples: number of trees (n_estimators), tree depth (max_depth), learning rate, regularization strength.

In short: Parameters = learned. Hyperparameters = chosen.

When would you choose Grid Search over Random Search, and vice‑versa? Grid Search
Use it when:
The search space is small

You want to evaluate every combination

You care about systematic, exhaustive exploration

Random Search
Use it when:

The search space is large

You want faster results

You suspect only a few hyperparameters matter

You want to explore a wider range without training hundreds of models

In practice: Grid Search = thorough but slow. Random Search = faster and often finds better results in high‑dimensional spaces.

Looking at the AutoGluon leaderboard, which model performed the best? What makes AutoML so powerful compared to manual tuning? The top row of the leaderboard shows the best-performing model (often a stacked ensemble or a boosted tree model like LightGBM).
AutoML is powerful because it:

Tries many model families automatically

Tunes hyperparameters for each model

Performs feature engineering

Builds ensembles that outperform individual models

Allocates time intelligently to the most promising approaches

In short: AutoML automates the entire modeling pipeline and often discovers combinations that humans would never try manually.
