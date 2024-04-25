# PrimateVision.DeepL


This repository presents custom implementations of the VGG16 and VGG19 convolutional neural network architectures for the classification of monkey species using the 10 Monkey Species dataset.

## Dataset

The 10 Monkey Species dataset comprises images of 10 distinct species of monkeys. Each image is tagged with one of the following species:

- 'n0': 'mantled_howler'
- 'n1': 'patas_monkey'
- 'n2': 'bald_uakari'
- 'n3': 'japanese_macaque'
- 'n4': 'pygmy_marmoset'
- 'n5': 'white_headed_capuchin'
- 'n6': 'silvery_marmoset'
- 'n7': 'common_squirrel_monkey'
- 'n8': 'black_headed_night_monkey'
- 'n9': 'nilgiri_langur'

## Implementation Details

### VGG16 Project

The VGG16 project employs the VGG16 architecture for image classification tasks.

- **Optimizer Used**: Adam optimizer
- **Loss Function**: Categorical cross-entropy
- **Layers Used**: Multiple convolutional layers with 3x3 filters, followed by max-pooling layers to downsample the feature maps. Fully connected layers with dropout regularization are used for classification.
- **Regularization Used**: L2 regularization with a regularization parameter of 0.01 applied to the dense layers.
- **Data Augmentation**: Techniques such as random rotations, shifts, flips, and zooms are applied during training to enhance model robustness.

#### Performance Metrics

- Train Loss: 0.2116 | Train Accuracy: 98.27%
- Validation Loss: 0.4009 | Validation Accuracy: 94.85%
- Test Loss: 0.4911 | Test Accuracy: 91.18%

### VGG19 Project

The VGG19 project utilizes the VGG19 architecture for image classification tasks.

- **Optimizer Used**: Nadam optimizer
- **Loss Function**: Categorical cross-entropy
- **Layers Used**: Multiple convolutional layers with 3x3 filters, followed by max-pooling layers to downsample the feature maps. Global average pooling layers are included to reduce spatial dimensions before dense layers with dropout regularization for classification.
- **Regularization Used**: L2 regularization with a regularization parameter of 0.001 applied to the dense layers.
- **Data Augmentation**: Similar data augmentation techniques are applied as in the VGG16 project.

#### Performance Metrics

- Train Loss: 0.3599 | Train Accuracy: 98.72%
- Validation Loss: 0.4815 | Validation Accuracy: 93.38%
- Test Loss: 0.6433 | Test Accuracy: 89.71%

---

This README provides comprehensive details about the monkey species classification projects utilizing the VGG16 and VGG19 architectures, including model configurations, optimization techniques, performance metrics, and more.
