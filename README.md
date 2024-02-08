# Deep Generative Models for Dehazing Satellite Images

### Abstract
Remote Sensing (RS) is the process of observing and measuring the physical features of an area from a distance by monitoring its reflected and emitted radiation, usually from a satellite or aircraft. The application of RS spans a wide range of fields, including precision agriculture, disaster management, military operations, environmental monitoring, and weather assessment, among others. Haze or pollution in the satellite images, makes satellite images unsightly and makes valuable information useless. Sometimes satellites must capture images in hazefilled atmospheres, rendering them unusable for study. This proposed work is implemented using the Modern Deep Learning techniques to dehaze the satellite images. We have proposed two GAN architectures, INC-Pix2Pix and RNX-Pix2Pix. A publicly available dataset was used for training our proposed approaches. To eliminate haze from images, we have suggested Deep Generative models by employing the best developments in the field of image processing. By using generative models, images can be dehazed without information loss, supporting the project's objective. It has the capacity to learn any kind of underlying data distribution using its learning mechanism. Therefore, it can dehaze satellite images that have been corrupted by haze. Existing systems can be made more efficient by integrating this approach.

### DL Models Proposed in this work
- **Inc-Pix2Pix (Inception Pix2Pix)** : Traditional Pix2Pix Network with the benifits of Inception Network running parallel to Generator (U-Net) of the GAN
- **RNX-Pix2Pix (ResNext Pix2Pix)** : Traditional Pix2Pix Network with the benifits of ResNext blocks in the bottle next of Generator (Encoder-Decoder) of the GAN

### Results

<table>
    <tr>
        <th rowspan=2>Model</th>
        <th colspan=2>Thin Haze</th>
        <th colspan=2>Moderate Haze</th>
        <th colspan=2>Thick Haze</th>
    </tr>
    <tr>
        <th>SSIM</th>
        <th>PSNR</th>
        <th>SSIM</th>
        <th>PSNR</th>
        <th>SSIM</th>
        <th>PSNR</th>
    </tr>
    <tr>
        <td>DCP</td>
        <td>0.724</td>
        <td>12.77</td>
        <td>0.573</td>
        <td>9.78</td>
        <td>0.585</td>
        <td>8.58</td>
    </tr>
    <tr>
        <td>DehazeNet</td>
        <td>0.895</td>
        <td>19.75</td>
        <td>0.855</td>
        <td>18.12</td>
        <td>0.706</td>
        <td>14.33</td>
    </tr>
    <tr>
        <td>SAR-OPT-CGAN</td>
        <td>0.841</td>
        <td>20.19</td>
        <td>0.794</td>
        <td>21.66</td>
        <td>0.757</td>
        <td>19.65</td>
    </tr>
    <tr>
        <td>B.Huang</td>
        <td>0.906</td>
        <td>24.16</td>
        <td>0.926</td>
        <td>25.31</td>
        <td>0.864</td>
        <td>25.07</td>
    </tr>
    <tr>
        <td>SkyGAN</td>
        <td>0.924</td>
        <td>25.38</td>
        <td>0.903</td>
        <td>25.58</td>
        <td>0.892</td>
        <td>23.43</td>
    </tr>
    <tr>
        <td>H2RL-Net</td>
        <td>0.929</td>
        <td>25.84</td>
        <td>0.928</td>
        <td>26.15</td>
        <td>0.901</td>
        <td>25.2</td>
    </tr>
    <tr>
        <td>Mo-GAN</td>
        <td>0.926</td>
        <td>25.47</td>
        <td>0.9176</td>
        <td>25.93</td>
        <td>0.899</td>
        <td>25.12</td>
    </tr>
    <tr>
        <td><b>RNX-Pix2Pix</b></td>
        <td>0.921</td>
        <td>22.27</td>
        <td>0.928</td>
        <td>23.01</td>
        <td>0.89</td>
        <td>21.46</td>
    </tr>
    <tr>
        <td><b>INC-Pix2Pix</b></td>
        <td>0.954</td>
        <td>25.55</td>
        <td>0.949</td>
        <td>26.25</td>
        <td>0.917</td>
        <td>23.33</td>
    </tr>
</table>

**Note:** Our Novel approaches have outperformed existing models.

### Other possible Approaches
- Due to Lack of Computation time cycle Gan models have been less emphasized though implemented.
- **RNX-CycleGAN** : In the traditional CycleGAN instead of the normal residual blocks resnext blocks have been used.
