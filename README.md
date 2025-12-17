# AutoEncoder
This project explores the implementation and application of autoencoders and related deep learning models using the Fashion-MNIST dataset — a collection of 28×28 grayscale images across 10 fashion categories. The core objective is to demonstrate unsupervised learning for tasks such as image reconstruction, noise reduction, and feature extraction.

The study begins with a standard autoencoder, consisting of an encoder that compresses input images into a compact latent representation (64 dimensions) and a decoder that reconstructs the original images. The model is trained using the Adam optimizer and binary cross-entropy loss over 50 epochs, achieving effective reconstruction and meaningful latent feature learning.

Next, the project introduces noise reduction using a denoising autoencoder. Synthetic Gaussian noise is added to the input images, and a simplified autoencoder is trained to recover the clean versions, successfully demonstrating the model's ability to remove noise and restore image quality.

Finally, the project extends into variational autoencoders (VAEs), which learn a probabilistic latent space. After training the VAE for stable reconstruction, its encoder is used as a feature extractor to train a separate classifier. The classifier — built with dense layers, batch normalization, and dropout — achieves around 84% accuracy on the test set, highlighting the effectiveness of VAE-learned features for downstream supervised tasks like image classification.

Overall, this project illustrates the versatility of autoencoder-based architectures in unsupervised representation learning and their practical utility in tasks ranging from denoising to feature-based classification.
