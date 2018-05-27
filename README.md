# Style Transfer by GANs
Neuron network project for converting between Apple-style and Windows-style emojis by training the CycleGAN.

The basic idea is to use a conditional GAN to learn a mapping from input to output images.
The loss functions of these approaches generally include extra terms
to express constraints on the types of images that are generated.

CycleGAN allows us to use un-paired training data

This means that in order to train it to translate images from domain X to domain Y,
we do not have to have exact correspondences between individual images in those domains.
For example, in the paper that introduced CycleGANs, the authors are able to translate
between images of horses and zebras, even though there are no images of a zebra
in exactly the same position as a horse, and with exactly the same background.

CycleGANs enable learning a mapping from one domain X (say, images of horses) to
another domain Y (images of zebras) without having to find perfectly matched training pairs.

Machine Learning Framework: PyTorch
