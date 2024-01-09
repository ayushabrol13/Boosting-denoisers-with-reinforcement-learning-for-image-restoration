## Abstract 

Learning-oriented techniques for image restoration typically involve teaching systems how to convert flawed
images into clean ones. Many existing methods concentrate on creating diverse deep neural network struc-
tures and innovative loss functions to address multiple mixed distortions with unknown proportions. Despite
their success in restoring images, these methods demand costly training data and generate outcomes that
lack interpretability. Our study introduces a novel approach utilizing deep reinforcement learning (DRL)
to repair distorted images. We frame the image restoration challenge as a Partially Observable Markov
Decision Process (POMDP), where actions correspond to various pixel-level image denoising operations. In
our method, individual agents handle pixels, learning to adjust their respective values by selecting appro-
priate combinations of actions. Additionally, we introduce an innovative exploration strategy that ensures
similar actions hold similar value, preventing overfitting during estimation of state-action values. Through
comprehensive experiments, we demonstrate our method’s efficacy in restoring images with multiple com-
bined distortions, showcasing comparable or superior performance to prior learning-based approaches. By
visualizing the weighting process of multiple pixel-level operations, we can discern the operation combina-
tions employed for each pixel at each stage. This advancement represents a stride toward enhancing the
explainability and interpretability of learning-based image restoration method.

## Objective

This Bachelor of Technology project aims to implement a novel method for image denoising using deep
reinforcement learning, which casts the image denoising problem as a Partially Observable Markov Decision
Process (POMDP) and allows for multiple pixel-wise image denoising operations. We aim to demonstrate
the effectiveness of our approach through extensive experiments and show that it performs comparably or
better than previous learning-based approaches. Additionally, We aim to contribute to the explainability and
interpretability of learning-based image denoising methods by visualizing the process of weighting multiple
pixel-wise operations.
The specific goals of the project are outlined as follows:
 - Reconceptualizing Restoration as a Multi-Agent Reinforcement Learning Problem: The
project redefines the challenge of multi-noise image restoration by framing it as a Multi-Agent Rein-
forcement Learning (MARL) problem under Partially Observable Markov Decision Process (POMDP),
providing a novel perspective to address image restoration.
 - Continuous Action Space for Pixel-Wise Restoration: Introduces a groundbreaking methodol-
ogy that operates in a continuous action space for pixel-wise image restoration. This approach sidesteps
the limitations of discrete action space methods, allowing for more precise and nuanced pixel-level ad-
justments.
 - Integrated Denoising Methodology with Traditional Filters: Proposes an integrated denoising
method that concurrently applies multiple traditional image filters to the noisy image. Then, a deep
reinforcement learning algorithm learns the optimal weight synthesis for fusing these filtered images
into a clearer restoration, enhancing restoration effectiveness.
 - Addressing Challenges of State Information in POMDP: Tackles the challenge of insufficient
state information in POMDP frameworks, offering solutions specifically addressing the deterministic
policy gradient method’s limitations within the continuous action space.
 - Toolbox and Agent Framework: The proposed method comprises two main components:
a toolbox housing various traditional image filters and an agent dynamically selecting actions to modify
pixel weights for these filters. This dual-framework design aims to achieve superior restoration results
by leveraging the strengths of both components.
