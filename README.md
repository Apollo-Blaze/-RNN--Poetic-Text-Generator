# Poetic Text Generator

## Overview
This project uses a Recurrent Neural Network (RNN) to generate poetic text based on the works of Shakespeare. The model is built using TensorFlow and Keras, and it generates new text sequences that mimic Shakespeare's style.

## Features
- **Text Preprocessing**: Converts Shakespeare's text into a format suitable for training the RNN.
- **Model Training**: Uses an LSTM-based RNN to learn the patterns in the text.
- **Text Generation**: Generates new text sequences based on the trained model.

## Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/Apollo-Blaze/poetic-text-generator.git
    ```
2. Navigate to the project directory:
    ```bash
    cd poetic-text-generator
    ```
3. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## Usage
1. Download the Shakespeare text file:
    ```python
    filepath = tf.keras.utils.get_file('shakespeare.txt', 'https://storage.googleapis.com/download.tensorflow.org/data/shakespeare.txt')
    ```
2. Train the model:
    ```python
    model.fit(x, y, batch_size=256, epochs=5)
    ```
3. Generate text:
    ```python
    print(generate_text(300, 0.5))
    ```

## Results
The model was trained for 5 epochs with the following loss values:

`Epoch 1`: 2.2293
`Epoch 2`: 1.6022
`Epoch 3`: 1.5029
`Epoch 4`: 1.4588
`Epoch 5`: 1.4244

## License
This project is licensed under the MIT License.
