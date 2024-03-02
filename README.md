# Object Removal and Impainting
Please refer to `object-removal-and-impainting.ipynb` notebook to see the fully documented and explained project.

## Abstract
Object removal/image inpainting is a natural and fundamental problem in Computer Vision, and this is for good reason too, as it is by no means an easy one. The objective of this project is to attempt to apply a conditional Deep Convolutional Generative Adversarial Network (cDCGAN) architecture to this problem, in the hopes that it would provide some good results.

The choice of GANs for this problem is well-motivated, as the assumption would be that the Generator network would generate reasonable inpaintings, and the Discriminator network would be able to discern between real images and generator-faked inpaintings.

To that purpose, we decided to apply the discussed techniques on the Sky dataset, where the GAN would attempt to remove the planes from the image, making the airspace appear clear. After many iterations and simplifying assumptions, we were able to develop a model that has some success with completing the task at hand, whereby the generator model is quite good at reconstructing the non-cropped portion of the image, but struggles to come up with a coherent filling for the cropped portion. It is clear to us that the problem we chose is much harder than we initially estimated, so we ended off with several remarks to consider for future improvements.

