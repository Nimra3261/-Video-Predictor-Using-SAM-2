# Video Predictor Using SAM 2

This project uses Facebook's Segment Anything Model (SAM) to perform video segmentation. The process involves mounting a Google Drive, setting up the environment, and executing the model on video frames to predict and segment objects.

## Project Structure

The project contains the following major steps:

1. **Environment Setup**:
   - Mount Google Drive.
   - Clone the `segment-anything-2` repository from GitHub.
   - Install necessary dependencies.

2. **Model Setup**:
   - Download the required model weights.
   - Set up the environment for running the segmentation model using `torch`.

3. **Video Segmentation**:
   - Load video frames.
   - Apply the SAM model to predict and segment objects in the video.
   - Visualize and save the segmented frames.

## Installation

### Prerequisites

- Python 3.7 or higher
- Google Colab environment (recommended for ease of use with Google Drive integration)
- GPU-enabled environment for faster processing (e.g., Google Colab with GPU runtime)

### Steps

1. **Mount Google Drive**:
    ```python
    from google.colab import drive
    drive.mount('/content/gdrive')
    ```

2. **Clone the GitHub Repository**:
    ```bash
    git clone https://github.com/facebookresearch/segment-anything-2.git
    cd /content/gdrive/MyDrive/segment-anything-2
    ```

3. **Install Dependencies**:
    ```bash
    pip install -e .
    ```

4. **Download Model Weights**:
    ```bash
    cd /content/gdrive/MyDrive/segment-anything-2/checkpoints/
    bash download_ckpts.sh
    ```

## Usage

1. **Change to Project Directory**:
    ```bash
    cd /content/gdrive/MyDrive/segment-anything-2/
    ```

2. **Run the Notebook**:
    Execute the cells in the notebook `VIdeo_Predictor_UsingSAM2.ipynb` to perform video segmentation.

3. **Output**:
    The segmented video frames are saved in the specified directory in your Google Drive.

## License

This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).

## Authors

This project was developed by me and is based on Facebook's Segment Anything Model (SAM).

