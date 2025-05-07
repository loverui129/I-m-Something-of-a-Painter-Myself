# I-m-Something-of-a-Painter-Myself
🖼️ Overview
This project applies a pretrained CycleGAN model to perform image-to-image translation from real-world photographs to Monet-style paintings. The task was inspired by the Kaggle competition "I'm Something of a Painter Myself", which challenges participants to generate visually convincing artistic renditions using GAN-based techniques.
We focused on reusing a pretrained generator (G_A2B) to conduct inference on a set of test photos, and generated stylized outputs in Monet’s aesthetic.

⚙️ Steps and Approach
1. Load Pretrained Generator
We initialized a ResNet-based generator (G_A2B) and loaded its saved .pth weights using PyTorch.

2.Set Up Inference Pipeline
We defined preprocessing transforms (resize, normalize, tensorize) consistent with the model's training.

Each test image was loaded, transformed, and passed through the generator to obtain the stylized output.

3. Generate Outputs
Output images were saved as .jpg files into a local images/ folder.

Finally, we zipped the folder as images.zip for submission to the competition.

4. Submission
The generated images.zip was submitted to Kaggle as the final inference result.
The notebook and pretrained weights were organized in a reproducible format for easy reruns and verification.

