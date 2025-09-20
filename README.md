# Traffic Sign Classifier

This project is about training an AI to **recognize traffic signs from images** — a core challenge in computer vision for self-driving cars. The model learns to classify road signs (stop, speed limit, yield, etc.) using supervised learning on the **German Traffic Sign Recognition Benchmark (GTSRB)** dataset.

## How It Works

* **Dataset:** 43 categories of road signs, thousands of labeled images.
* **Processing:** Images are loaded with OpenCV, resized to 30×30, and normalized.
* **Model:** A Convolutional Neural Network (CNN) built with **TensorFlow/Keras**.
* **Training:** Data is split into training/testing sets with **scikit-learn**.
* **Evaluation:** Accuracy is measured on the test set; models can be saved and re-used.

## Technologies Used

* **Python 3.11** (recommended)
* **TensorFlow/Keras** – neural networks
* **OpenCV** – image processing
* **scikit-learn** – data splitting and utilities

## Tree structure
```
TRAFFIC/
├── gtsrb/              # Dataset folder (traffic sign images by class)
├── .gitignore          # Git ignore rules
├── README.md           # Project documentation
├── requirements.txt    # Python dependencies
└── traffic.py          # Main training and evaluation script
```


## Running

1. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

2. Downloading and installing gtrsb dataset

```bash 
curl -L https://cdn.cs50.net/ai/2023/x/projects/5/gtsrb.zip -output gtsrb.zip
bsdtar -xf gtsrb.zip
rm gtsrb.zip
```

2. Train the model:

   ```bash
   python traffic.py gtsrb
   ```
---




