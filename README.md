# SA_capstone_project

📊 Visualizations & Model Comparison
This section compares the price evolution of both models using Bokeh plots, highlighting their behavior and effectiveness.


🔹 Model 1: Baseline Linear Pricing

Explanation:

1. The baseline linear model increases the parking price directly with occupancy ratio at each window.

2. Prices rise steeply during periods of rapid occupancy growth, which can lead to sudden spikes — like the sharp price jumps seen in early December.

3. This model is simple and responsive but lacks smoothing mechanisms, resulting in potential price volatility.

4. It demonstrates that a purely linear relationship can overreact when occupancy swings occur, causing prices to become erratic and possibly confusing or frustrating customers.



🔹 Model 2: Demand-Based Pricing

Explanation:

1. The demand-based model uses a composite demand function combining occupancy ratio, queue length, traffic congestion, special days, and vehicle type.

2. This approach normalizes the demand signal and adjusts prices within a bounded range (0.5x to 2x the base price), ensuring smooth and explainable price transitions.

3. Compared to Model 1, the pricing curve here is much more stable, avoiding erratic jumps while still reflecting genuine changes in demand.

4. Even during times of increased occupancy or special events, the demand function’s design dampens extreme price spikes, which leads to a better user experience and more predictable revenue.



🔎 Key Insights

✅ Baseline Model Strengths:

1. Simple and easy to implement.

2. Reacts immediately to changes in occupancy.

❌ Baseline Model Weaknesses:

1. Highly sensitive to short-term occupancy fluctuations.

2. Lacks consideration of other demand factors (queue, traffic, events).

✅ Demand-Based Model Strengths:

1. Incorporates multiple real-world signals into a holistic demand measure.

2. Maintains prices in a stable, controlled band — avoiding extreme volatility.

3. Produces pricing behavior that aligns with economic theory of supply-demand balance.

❌ Demand-Based Model Weaknesses:

1. Slightly more complex to implement and tune feature weights.

2. May require additional data engineering to preprocess features like traffic or event indicators.



📌 Conclusion

Including both models demonstrates a progression from a straightforward occupancy-driven approach (Model 1) to a richer, more robust demand-aware pricing system (Model 2). While the baseline provides a simple benchmark, the demand-based pricing offers smoother, more realistic pricing evolution suitable for dynamic urban parking environments.
