# Emotion-based Music Recommendation System

This project is an innovative application that combines facial emotion recognition with music recommendations. It captures the user's facial expressions through a webcam, determines their emotional state, and suggests music based on the detected emotion.

## Features

- Real-time facial emotion detection using a webcam
- Emotion classification into 7 categories: Angry, Disgusted, Fearful, Happy, Neutral, Sad, Surprised
- Music recommendations based on detected emotion
- Integration with Spotify API for accessing music data
- User-friendly GUI built with Tkinter

## Prerequisites

- Python 3.7+
- Webcam
- Spotify Developer account (for API access)

## Installation

1. Clone this repository:
   ```
   git clone https://github.com/yourusername/emotion-music-recommendation.git
   cd emotion-music-recommendation
   ```

2. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```

3. Download the pre-trained emotion recognition model (`model.h5`) and place it in the project root directory.

4. Set up your Spotify API credentials:
   - Create a Spotify Developer account and create a new application
   - Set your Client ID and Client Secret as environment variables:
     ```
     export SPOTIPY_CLIENT_ID='your-spotify-client-id'
     export SPOTIPY_CLIENT_SECRET='your-spotify-client-secret'
     ```

## Usage

Run the main application:

```
python main.py
```

The application will open a GUI window. Grant permission to access your webcam when prompted. The system will start detecting your facial expression and recommending music based on your emotional state.

## Project Structure

- `main.py`: The main application script
- `utils.py`: Utility functions for webcam streaming
- `haarcascade_frontalface_default.xml`: Haar Cascade classifier for face detection
- `model.h5`: Pre-trained emotion recognition model
- `requirements.txt`: List of Python dependencies
- `songs/`: Directory containing CSV files with song recommendations for each emotion

## Technologies Used

- TensorFlow and Keras for the emotion recognition model
- OpenCV for image processing and face detection
- Spotipy for Spotify API integration
- Pandas for data manipulation
- Tkinter for the graphical user interface

 ## Research Basis
This project is inspired by and builds upon the research presented in the paper: \
“A Novel Emotion-based Music Recommendation System using CNN”, 2023 7th International Conference on Intelligent Computing and Control Systems (ICICCS), Madurai, India, 2023

https://www.researchgate.net/publication/371430777_A_Novel_Emotion_based_Music_Recommendation_System_using_CNN

This paper proposes a novel approach to emotion-based music recommendation using Convolutional Neural Networks (CNN), which aligns closely with the methodology used in our project. We encourage interested users and contributors to read this paper for a deeper understanding of the theoretical foundations of our system.


## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

