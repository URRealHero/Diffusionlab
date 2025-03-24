# Lab2's goal
1. Get to know how we construct the training target, in this lab, the $p_{data}$ is manually defined as  
$$p_{data} = GaussianMixture.symmetric_{2D}(nmodes=5, std=1.0, scale=10.0)$$
2. $x_0$ from $p_{init}=Gaussian.isotropic(dim=2, std = 1.0)$
3. Entire Pipeline(flow matching as an example)
   1. Sample a data(z) from $p_{data}$
   2. Use this z, we can construct a probability path (Manually designed Linear $\alpha_t$ and sqrt $\beta_t$)
   3. Probability path -> we can get the conditional vector field with formula
   4. Now, we can construct the Conditional Vector Field ODE to numerically simulate(with delta t)
   5. Lastly, we get the simulation trajectory for single data point z.
4. Section 3: