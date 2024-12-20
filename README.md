# Denoising Images with a Convolutional Autoencoder

## Brief Description of the Task
Autoencoders can be used to denoise images by learning to reconstruct clean, noise-free versions of noisy images. The network consists of two parts: the encoder, which compresses the noisy input into a lower-dimensional representation (latent space), and the decoder, which reconstructs the original image from this compressed encoding. During training, the autoencoder is fed noisy images as inputs and the corresponding clean images as targets. By minimizing the difference between the noisy input and the reconstructed output, the autoencoder learns to filter out the noise, effectively denoising the images. Once trained, the model can remove noise from unseen noisy images by passing them through the encoder-decoder network.

## Hyperparameters

The following table summarizes the hyperparameters used for training the convolutional autoencoder:

| Hyperparameter      | Value        |
|---------------------|--------------|
| **Epochs**          | 15           |
| **Optimizer**       | Adam         |
| **Learning Rate (lr)** | 1e-3      |
| **Weight Decay**    | 1e-5         |
| **Batch Size**      | 64           |


## LResults

The table below shows the final average training and testing losses after completing the training:

| Loss Type          | Final Value  |
|--------------------|--------------|
| **Avg Train Loss** | 0.05094      |
| **Avg Test Loss**  | 0.05097      |

