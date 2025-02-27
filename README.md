# **Neural Style Transfer**

**Objective:** Implement the NST algorithm from *Gatys et al. (2015)* to merge a content image (e.g., the Louvre Museum) with a style image (e.g., a Monet painting) using a pretrained convolutional neural network (CNN), VGG-19.

**Key Components:**
- **Content Cost:** Measures how well the generated image preserves the content of the content image using activations from a middle layer of VGG-19.
- **Style Cost:** Quantifies how well the generated image captures the style of the style image using Gram matrices from multiple VGG-19 layers.
- **Total Cost:** Combines content and style costs with weights (alpha and beta) to optimize the generated image’s pixels directly.
- **Optimization:** Uses gradient descent to update pixel values, not network weights, which is a unique twist compared to typical deep learning tasks.

**Process:** Loads a pretrained VGG-19, computes content and style costs, and iteratively optimizes a generated image starting from random noise or the content image.

**Output:** Generates an artistic image, with examples like the Louvre in Monet’s style, and provides options to test custom images.

![image](https://github.com/user-attachments/assets/822d2d0a-cb14-4042-8b1b-610d3afa1c9a)
