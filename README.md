# Balance Postures Dataset

This repository contains a dataset created to classify balance tests from the Short Physical Performance Battery (SPPB), with classes for *feet-together*, *semi-tandem*, *tandem*, and a fourth class called *no-balance*, representing any other posture different from the previous three. This dataset is intended for use in computer vision models and applications in health and biomechanics.

## Dataset Content

The dataset includes a total of 800 images, captured from 20 individuals, distributed into training and test folders:
- **Training**: 640 images, 10 per class for each of 16 individuals.
- **Testing**: 160 images, 10 per class for each of 4 individuals.

### Balance Classes:

- **Feet Together**
- **Semi-Tandem**
- **Tandem**
- **No Balance**

### Image Resolution

- **Original Resolution**: 720x1280 pixels.
- **Resized Version**: 224x224 pixels.


Each main folder (train, test, train224, test224) contains subfolders for each of these classes, organized as follows:

```plaintext
balance-postures-dataset/
├── train/          # Training images (original)
│   ├── feet-together/
│   ├── semi-tandem/
│   ├── tandem/
│   └── no-balance/
├── test/           # Testing images (original)
│   ├── feet-together/
│   ├── semi-tandem/
│   ├── tandem/
│   └── no-balance/
├── train224/       # Training images (224x224)
└── test224/        # Testing images (224x224)
```

## Usage

1. **Clone the repository**:
   ```bash
   git clone https://github.com/agascocompte/balance-postures-dataset.git
   ```
2. **Load and process**: The dataset is ready to be loaded and processed in deep learning frameworks such as PyTorch or TensorFlow, either in its original size or in the 224x224 version.

## Applications

- Image-based balance classification models.
- Research in fall prevention and balance analysis.

## License

This project is licensed under the MIT License.
