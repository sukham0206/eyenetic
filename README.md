# Eyenetic : Eye-Controlled Movement

Eyenetic is a prototype designed to empower physically disabled individuals who are unable to walk and rely on wheelchairs for mobility. The primary objective of this project is to enable wheelchair control through eye movements. By utilizing cutting-edge technology, Eyenetic allows users to operate their wheelchairs effectively using their eyes.

## Project Overview

The purpose of Eyenetic is to provide a solution for people who face mobility challenges due to physical disabilities. By harnessing the power of eye-tracking technology, this project aims to offer an innovative and accessible method for controlling wheelchairs.

## Key Features

- **Eye Movement Detection**: Eyenetic utilizes a Convolutional Neural Network (CNN) that has been trained on a custom dataset of approximately 1000 images capturing various eye movement directions.

- **Mouse Pointer Control**: The trained CNN accurately detects the user's eye movements and translates them into corresponding mouse pointer movements on a screen.

- **Wheelchair Integration**: The mouse pointer's movements can be seamlessly integrated with the control system of an electric wheelchair, allowing users to navigate their environment efficiently.

## How it Works

1. **Data Collection**: A unique dataset of eye images in different directions is recorded to facilitate the training of the CNN. This dataset forms the foundation for accurately identifying distinct eye movements.

2. **CNN Training**: A Convolutional Neural Network is employed to learn and recognize patterns within the eye images. Through iterative training, the CNN becomes proficient in detecting specific eye movement patterns.

3. **Eye Movement Detection**: Once trained, the CNN can swiftly identify the direction in which the user's eyes are moving. This information is then used to control the movement of a mouse pointer on a screen.

4. **Mouse Pointer Control**: The mouse pointer's movement, determined by the user's eye movements, can be connected to an electric wheelchair's control system. This enables the user to navigate the wheelchair simply by moving their eyes.

## Getting Started

To use Eyenetic, follow these steps:

1. **Dataset**: Make sure you have a diverse dataset of eye images capturing various eye movement directions. This dataset will be used for training the CNN.
Run the python script using ``python ds.py`` and create the dataset by clicking on various parts of your monitor and looking in the respective direction.

2. **CNN Training and Integration**: Train a Realtime Convolutional Neural Network by typing ```python model.py``` using the dataset to enable accurate eye movement detection. Various deep learning frameworks such as TensorFlow or PyTorch can be utilized for this purpose.


## Future Enhancements

Eyenetic has the potential for various future enhancements:

As this was just a prototype, the images of the eyes used were of very low resolution (32x32) and the dataset was manually collected which accounted for only 1000 images
The future updates of eyenetic would focus on the following:

- Using a better device for dataset collection (something like a phone camera).
- Increasing the post cropping resolution of the captured images and collecting a larger dataset.
- Updating the model architecture to handle the higher resolution images.
- Integrating the model with actual electric wheelchairs



