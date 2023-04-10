# Wildfire Risk Prediction and Burn Scar Segmentation App
This repository contains a Streamlit app that uses two different deep learning models. The first model is a Convolutional Neural Network (CNN) trained on satellite images to predict whether an area is at risk of a wildfire or not. The second model is a SegNet model trained to segment burn scars caused by wildfires in satellite images.

## Data
The data used in this project for wildfire prediction is satellite images obtained from Mapbox API. The images used for burn scar segmentation are obtained from another source and are annotated with burn scar masks.

## Models
### Wildfire Risk Prediction Model
The wildfire risk prediction model is a CNN trained on satellite images to predict whether an area is at risk of a wildfire or not. The model takes as input a latitude and longitude coordinate and outputs a probability of the area being at risk of a wildfire.

### Burn Scar Segmentation Model
The burn scar segmentation model is based on the SegNet architecture, which is an encoder-decoder architecture that uses convolutional and pooling layers in the encoder to extract features from the input image and upsampling and deconvolution layers in the decoder to recover the original image resolution. The model is trained using annotated satellite images and is used to create a mask of the burn scars in the image.

## App
The app allows users to choose between the two models: wildfire risk prediction or burn scar segmentation. For the wildfire risk prediction model, users can input the latitude and longitude coordinate of the area they are interested in and the app will output a probability of the area being at risk of a wildfire. For the burn scar segmentation model, users can upload a satellite image and see the burn scar segmentation.

- To run the app locally, follow these steps:

1. Clone this repository using the command:
git clone https://github.com/abdouaaba/wildfire_system_app.git

2. Install the required packages:
pip install -r requirements.txt

3. Run the app using the command:
streamlit run app.py

- Link to the app on Streamlit Cloud
[Wildfire system app](https://abdouaaba-wildfire-system-app-app-8ki3hv.streamlit.app/)

## Credits
The wildfire risk prediction model is trained using the [wildfire-prediction](https://github.com/abdouaaba/wildfire-prediction) repository.

The burn scar segmentation model is trained using the [wildfire-burn-scars-segmentation](https://github.com/abdouaaba/wildfire-burn-scars-segmentation) repository.
