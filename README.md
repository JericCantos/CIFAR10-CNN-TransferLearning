# CIFAR10-CNN-TransferLearning
A comparison transfer learning models (ResNet50-based) and custom CNN performance on classifying images from the CIFAR10 database.

## notebooks
`CIFAR_10_Image_Classification.ipynb` contains the model architecture, training, and performance analysis.

## models
The best performing (and most time-consuuming) model was saved as `custom_cnn.keras`. It could be reloaded using the following code snippet:

```
import os
from tensorflow.keras.models import load_model

save_dir = 'DIRECTORY_CONTAINING_FILE' # e.g. /content/drive/MyDrive/Masterschool_Computer_Vision/'

model_path = os.path.join(save_dir, 'custom_cnn.keras')
custom_cnn = load_model(model_path)
```