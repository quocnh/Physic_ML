# physic_ml
- An mode decomposition based CNN Autoencoder. Please check the report for more information.


### Nonlinear Feature Extraction:


Traditional methods like POD (Proper Orthogonal Decomposition) are linear and struggle with highly nonlinear problems like high Reynolds number flows
The paper demonstrates that CNN autoencoders with nonlinear activation functions (like tanh) can capture nonlinear features better than linear methods
For example, with POD, 7260 modes are needed to reproduce 95% of total energy for a turbulent channel flow, while CNN autoencoders can achieve good reconstruction with fewer modes


### Dimensionality Reduction:


The autoencoder compresses high-dimensional flow field data into a low-dimensional latent space (2 dimensions in their examples)
This allows efficient representation and storage of complex flow dynamics using much less data
The low-dimensional representation still preserves important flow features and can accurately reconstruct the original flow field


### Visualization and Interpretability:


The paper introduces a new "Mode Decomposing CNN Autoencoder" (MD-CNN-AE) that can visualize individual flow modes
This helps understand what features the network learns, making it more interpretable than standard CNN autoencoders
The decomposed modes provide physical insights into the flow structures


### Computational Efficiency:


Using the compressed latent representation saves computational resources
The paper mentions CNN's "weight sharing" concept allows handling large fluid datasets efficiently
Once trained, the model can quickly encode new flow fields into low-dimensional representations

![viewer](https://github.com/quocnh/physic_ml/blob/main/comprarison_mode.png)
