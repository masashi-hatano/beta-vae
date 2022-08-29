# $\beta$-VAE
## Image generation of MNIST via Beta-VAE

In this repository, we implementaed $\beta$-Variational AutoEncoder using CNN architecture.
The effect of introducing the coefficient of $\beta$ in the regularization term of loss function can be seen.

## Visualization of manifolds in latent space
In the case of $\beta$ is equal to two or four, the disentanglement of the model is better than when $\beta$ is equal to one; however, if the coefficient is too large, $\beta$ is 20, the model cannot reconstruct images. This is because KL divergence contains the factor of mutual information between input $x$ and latent variable $z$, and if mutual information goes to zero, information of input cannot be encoded well.

### $\beta$=1:
![manifolds_beta=1](https://user-images.githubusercontent.com/71377772/187130915-0710f257-c149-48a8-855a-b7d6eaed1d20.png)
### $\beta$=2:
![manifolds_beta=2](https://user-images.githubusercontent.com/71377772/187131021-f16f7eca-04cc-4901-8e4b-d673ab7f888e.png)
### $\beta$=4:
![manifolds_beta=4](https://user-images.githubusercontent.com/71377772/187131079-24d8046b-4c63-4634-a033-c93d43767d77.png)
### $\beta$=10:
![manifolds_beta=10](https://user-images.githubusercontent.com/71377772/187131098-c7f06a0e-d54f-4886-b519-530651f67297.png)
### $\beta$=20:
![manifolds_beta=20](https://user-images.githubusercontent.com/71377772/187131119-46f59a03-5af1-41fd-8615-a3a743f68803.png)
