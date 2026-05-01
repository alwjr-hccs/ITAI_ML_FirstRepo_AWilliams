Which model is underfitting, which is overfitting, and which is a good fit? Why? Degree 1 → Underfitting
The model is too simple (just a straight line). It cannot capture the curvature of the sine wave, so both the training and validation errors remain high. This is classic high bias.
Degree 4 → Good Fit
The model captures the smooth oscillation of the sine wave without chasing noise. It generalizes well and visually aligns with the underlying pattern. This is the bias–variance sweet spot.

Degree 15 → Overfitting
The model bends aggressively to match every wiggle in the noisy data. It fits the training data extremely well but produces unrealistic oscillations. This is high variance.

What do you observe in the learning curve for the underfitting model? What does it tell you? Both training and cross‑validation scores are low.
The two curves sit close together.

Adding more data does not significantly improve performance.

This tells you the model is too simple to capture the underlying pattern. The problem is high bias, not lack of data.

What do you observe in the learning curve for the overfitting model? What does it tell you? The training score is extremely high (near perfect).
The cross‑validation score is much lower.

There is a large, persistent gap between the curves.

Even with more data, the gap does not close fully.

This tells you the model is overfitting — it memorizes the training data but fails to generalize. The problem is high variance, not insufficient training.
