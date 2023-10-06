# Deep Generative Models for Dehazing Satellite Images

### Abstract
Remote Sensing (RS) is the process of observing and measuring the physical features of an area from a distance by monitoring its reflected and emitted radiation, usually from a satellite or aircraft. The application of RS spans a wide range of fields, including precision agriculture, disaster management, military operations, environmental monitoring, and weather assessment, among others. Haze or pollution in the satellite images, makes satellite images unsightly and makes valuable information useless. Sometimes satellites must capture images in hazefilled atmospheres, rendering them unusable for study. This proposed work is implemented using the Modern Deep Learning techniques to dehaze the satellite images. We have proposed two GAN architectures, INC-Pix2Pix and RNX-Pix2Pix. A publicly available dataset was used for training our proposed approaches. To eliminate haze from images, we have suggested Deep Generative models by employing the best developments in the field of image processing. By using generative models, images can be dehazed without information loss, supporting the project's objective. It has the capacity to learn any kind of underlying data distribution using its learning mechanism. Therefore, it can dehaze satellite images that have been corrupted by haze. Existing systems can be made more efficient by integrating this approach.

### DL Models Proposed in this work
- **Inc-Pix2Pix (Inception Pix2Pix)** : Traditional Pix2Pix Network with the benifits of Inception Network running parallel to Generator (U-Net) of the GAN
- **RNX-Pix2Pix (ResNext Pix2Pix)** : Traditional Pix2Pix Network with the benifits of ResNext blocks in the bottle next of Generator (Encoder-Decoder) of the GAN

### Other possible Approaches
- Due to Lack of Computation time cycle Gan models have been less emphasized
- **RNX-CycleGAN** : In the traditional CycleGAN instead of the normal residual blocks resnext blocks have been used.
