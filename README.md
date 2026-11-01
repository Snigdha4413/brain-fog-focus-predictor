# Focus Forecast 

**Focus Forecast** is a lightweight, fully client-side neural network application built in a single HTML file. It predicts your cognitive energy and focus level throughout the day based on lifestyle factors (sleep, hydration, screen time, caffeine, stress, and meeting load) and fine-tunes itself on your personal daily logs.

No heavy Python backends, external APIs, or heavy ML frameworks required—just pure JavaScript implementing a feedforward neural network running directly in your browser.

---

## Features

- **Built-in Neural Network:** A 2-hidden-layer dense neural network ($10 \rightarrow 16 \rightarrow 8 \rightarrow 1$) written in vanilla JavaScript featuring ReLU activations, dropout regularization, and stochastic gradient descent (SGD) optimization.
- **Synthetic Pre-Training:** Instantly pre-trains on simulated data featuring complex non-linear interactions (e.g., compounding effects of sleep deprivation combined with high screen time and low hydration) so it works right out of the box.
- **Personalized Fine-Tuning:** After logging 5 days of actual data, the model fine-tunes its weights on your personal inputs to adapt to your unique biological baseline.
- **Counterfactual "What-If" Analysis:** Instantly calculates how small lifestyle tweaks (e.g., drinking an extra liter of water, cutting 150mg of caffeine, or sleeping 1 hour more) will impact your predicted focus score.
- **Local Persistence:** Saves your training state and history securely in your browser's `localStorage`.

---

## Project Structure

```text
focus-forecast/
└── Focus Forecast.html    # Contains the complete HTML, CSS, and JS application
└── README.md              # Project documentation
