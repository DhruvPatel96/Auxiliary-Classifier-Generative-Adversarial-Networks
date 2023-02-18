# Auxiliary-Classifier-Generative-Adversarial-Networks

Fake Anime Face Generation using ACGAN
This is a project that uses Adversarial Conditional Generative Adversarial Networks (ACGANs) to generate realistic fake anime faces. The model is trained on a dataset of anime faces using the PyTorch deep learning framework.

Dataset
The dataset used in this project is the Anime Face Dataset from bchao1, which contains over 63,000 anime face images. The dataset is loaded using the opendatasets package and transformed into PyTorch ImageFolder format using torchvision.transforms.

Model Architecture
The ACGAN consists of two separate networks - a generator and a discriminator - that are trained together. The generator takes a random noise vector and a categorical label as input and outputs a fake anime face. The discriminator takes a real or fake anime face and a categorical label as input and outputs a probability score indicating whether the image is real or fake.

Training
The model is trained using a custom training loop with torch.utils.data.DataLoader. The generator and discriminator are trained in alternating batches, with the discriminator trying to distinguish between real and fake images while the generator tries to generate more realistic fake images that fool the discriminator. The training progress is visualized using tqdm and matplotlib.pyplot.

Results
After training for a certain number of epochs, the generator can produce fake anime faces that are visually indistinguishable from real ones. The generated images can be saved using torchvision.utils.save_image and visualized using matplotlib.pyplot.

Usage
To use this project, simply clone the repository and run the GANN.ipynb notebook. You can adjust the hyperparameters and the number of training epochs to see how it affects the generated images.
