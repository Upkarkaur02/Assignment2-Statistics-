Title: Learn Probability Density Functions using Roll-Number-Parameterized Non-Linear Model
1. Methodology
   ![ChatGPT Image Jan 31, 2026, 07_13_13 PM](https://github.com/user-attachments/assets/96ea7e02-2f31-48ef-94a3-2ea98eae97bb)
2. Description
  a.  Data Collection:
   The air quality dataset containing NO₂ concentration values was collected from Kaggle.
  b. Data Pre-Processing:
     The dataset was cleaned by removing missing and corrupted entries. The NO₂ feature was transformed using a roll-number-based non-linear transformation.
  c. PDF Parameter Estimation:
    A Gaussian-shaped probability density function was assumed for the transformed data. The parameters μ, λ, and c were estimated using Maximum Likelihood Estimation.
  d. Density Evaluation:
     The learned probability density function was evaluated for the transformed data points to model their distribution.
  e. Result Interpretation:
    The estimated parameters were analyzed, and the learned probability density function was visualized to validate the model.
3. Input/Output
   Input NO₂ Concentration Values from Dataset (x)
   -> Input University Roll no.
   -> Compute Transformation Parameters aᵣ = 0.05 × (r mod 7); bᵣ = 0.3 × (r mod 5 + 1)
   -> Apply Non-Linear Transformation z = x + aᵣ sin(bᵣ x)
   -> Input Transformed Values (z) to PDF Model
   -> Learn PDF Parameters(λ, μ, c) using Estimation Method
   -> Compute Predicted Probability Density p̂(z)
   -> Output Results • λ, μ, c • p̂(z) values
4. Live Link
   https://colab.research.google.com/drive/1gS7AKBCZ3bCScFQ4v2JwD19hiChSpsTL#scrollTo=XpY3L_qoOqAO
5. Screenshot
   <img width="746" height="225" alt="image" src="https://github.com/user-attachments/assets/c6369673-c44d-4b92-b614-6b25bc0f527b" />
