# Pre-shoplifting Detection with Faster R-CNN ResNet-50 V2 and RNN

This repository contains a TensorFlow implementation of Faster R-CNN with a ResNet-50 backbone, fine-tuned to detect shoplifting behaviors in video or image data.

## Key Features

- Utilizes a pretrained Faster R-CNN model with ResNet-50 backbone.
- Fine-tuned specifically for detecting shoplifting behaviors.
- Implements both object detection and temporal sequence analysis using RNN.

## Prerequisites

- Python 3.6+
- TensorFlow 2.x
- TensorFlow Hub
- PIL (for image and video processing)
- NumPy
- pandas
- venv

## Dataset

- **Source of the dataset**:
  - UCF-Crime dataset (Shoplifting Videos)
- **Data format**:
  - Videos

## Setup

1. **Clone the repo**

   ```sh
   git clone https://github.com/your_username/shoplifting-detection
   cd shoplifting-detection
   ```

2. **Install the requirements**

   Activate venv then

   ```sh
   pip install -r requirements.txt
   ```

3. **Update Directory Paths**

   - The code contains directory-specific file paths. Update the paths in the code to match your local directory structure.
   - Open the relevant scripts and modify the paths to point to the correct locations of your dataset and output directories.

   For example,

   ```python
   DATA_DIR = "/path/to/your/data/"
   FRAME_DIR = "/path/to/output/frame/directory"
   ```

   NOTE: DATA DIR Follows a 3 folder directory containing the videos

   ```
   shoplifting-detection/
   ├── data/
   │ ├── train/
   │ ├── validation/
   │ └── test/
   ```

4. **Run the code**
   - Ensure your dataset is properly formatted and placed in the specified directories.
   - Execute the notebook to start training or evaluating the model.

## References

- The UCF-Crime dataset can be accessed from [here](http://webpages.charlotte.edu/cchen62/dataset.html).
- For more information on Faster R-CNN, refer to the original paper [here](https://arxiv.org/abs/1506.01497).

## License

This project is licensed under the MIT License - see the LICENSE file for details.
