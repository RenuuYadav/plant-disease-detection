# 🌱 Plant Disease Detection


A machine learning-powered application to detect plant diseases from images. The system helps farmers and gardeners identify diseases early, leading to timely treatment and improved crop yield.


## 🌟 About the Project

This project aims to provide a reliable and accurate method to detect diseases in plants using image classification techniques. Leveraging deep learning models such as Convolutional Neural Networks (CNNs), we analyze images of plant leaves to identify if the plant is healthy or infected by a disease. The system can classify various types of plant diseases.

## 🚀 Features

- Image-based plant disease detection.
- Fast and efficient inference.
- Scalable and can be adapted to different types of plants and diseases.
- Web interface to upload images (React/Node.js).
- Mobile app integration for field usage (React Native).

## 📊 Dataset

We used the [PlantVillage dataset](https://www.plantvillage.org/), which consists of 50,000+ labeled images of healthy and diseased plant leaves. This dataset covers crops such as tomatoes, potatoes, apples, and others, with common diseases like:

- Apple Scab
- Powdery Mildew
- Late Blight
- Mosaic Virus

## ⚙️ Installation

To get the project up and running, follow these steps:

1. **Clone the repository**:
    ```bash
    git clone https://github.com/your-username/plant-disease-detection.git
    cd plant-disease-detection
    ```

2. **Install the required dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

3. **Download the dataset**:
    - Download the dataset from the [PlantVillage dataset link](https://www.plantvillage.org/).
    - Extract the dataset and place it in the `data/` directory.

4. **Train the model** (Optional):
    ```bash
    python train.py --dataset data/plant-disease
    ```

5. **Run the application**:
    - If you're using the web interface:
      ```bash
      python app.py
      ```
    - If you're using the mobile app:
      - Navigate to the `mobile/` directory and follow the React Native setup.

## 🚦 Usage

Once the application is running, you can use the following steps to detect plant diseases:

1. **Web App**:
   - Navigate to `http://localhost:5000`.
   - Upload a plant leaf image.
   - The model will analyze the image and return the result.

2. **Mobile App**:
   - Launch the React Native app.
   - Take a photo of the plant leaf or upload an image from your phone.
   - Get instant disease detection results.

## 🧠 Model Architecture

The project uses a **Convolutional Neural Network (CNN)** model trained on the PlantVillage dataset. The architecture involves:

- Input layer (RGB image).
- Several convolutional layers to extract features.
- Pooling layers for dimensionality reduction.
- Fully connected dense layers.
- Softmax output for multi-class classification.

You can modify and experiment with different architectures in the `model.py` file.

## 🤝 Contributing

We welcome contributions! Here's how you can contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/new-feature`).
3. Make your changes.
4. Commit the changes (`git commit -m 'Add some feature'`).
5. Push to the branch (`git push origin feature/new-feature`).
6. Open a Pull Request.
