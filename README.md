# Text To Song Generative System - Project "Vivy"

## Introduction
In recent years, Artificial intelligence has made significant strides in various domains, such as chatbot, self-driving, image generation, and music generation. In our project, we aim to develop a complete text-to-song system where users can input lyrics, song style, BPM, and other information to obtain a fully AI-generated, complete piece of music with synthesized singing voice. This is to further accelerate the application of AI in the field of art.  
Due to the substantial complexity of this project and time constraints during the development process, in this project, we have only developed the voice generation part. The rhythm generation and the creation of complete music will be implemented in the future.

## Features
- **Machine Learning Models**: Utilizing cutting-edge models for singing file (.ds) generation.
- **Vocal Synthesis**: Using DiffSinger to generate vocal.

## Getting Started
### Prerequisites
- Python 3.8 or later
- Dependencies listed in `requirements.txt`

### Installation
1. Clone the repository:
```
git clone https://github.com/nikmomo/Song-Generation-Model-with-Vocal-Project-Vivy.git
```

2. Install required packages:
```
pip install -r requirements.txt
```

### Usage
- **data**: All collected data are stores here.
- **DiffSinger**: State of art voice synthesis model.
- **lyric_data_processing.ipynb**: Process all data and provide *filtered dataset* and *normalzied dataset*.
    - *normalized_output.csv*: Normalized output file that used for training and validating the models.
    - *output.csv*: Dataset with filtered and aligned data.
- **model_training_RNN_LSTM.ipynb**: Training the model using RNN with LSTM.
- **model_training_RNN_GRU.ipynb**: Training the model using RNN with GRU.
- **model_training_Transformer.ipynb**: Training the model using Transformer.
- **musicgen_dmeo.ipynb**: MusicGen demo from audioCraft.
- **note_token_to_int.json**: The dictionary to convert notes to integers embedded format.
- **ph_token_to_int.json**: The dictionary to convert phoneme to integers embedded format.
- **note_scaler.pkl**: Scaling notes using MinMaxScaler.


## Examples
Predicting the result with input *Never gonna give you up, never gonna let you down.*  
See `predictions` for the prediction result

## License
This project is licensed under the MIT License - see the `LICENSE` file for details.
