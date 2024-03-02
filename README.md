# Audio Classification Project using Librosa

## Description

This GitHub repository contains an audio classification project using the Librosa library. The project focuses on classifying urban sounds into 10 classes:

1. Air Conditioner
2. Car Horn
3. Children Playing
4. Dog Bark
5. Drilling
6. Engine Idling
7. Gun Shot
8. Jackhammer
9. Siren
10. Street Music

The dataset used for this project consists of 8732 labeled sound excerpts (<=4s) sourced from field recordings on [Freesound](https://www.freesound.org/). The excerpts are pre-sorted into ten folds (folders named fold1-fold10) to facilitate reproduction and comparison with automatic classification results. For detailed information on the dataset compilation, refer to the accompanying paper.

## Dataset Contents

### Audio Files

- 8732 audio files of urban sounds in WAV format, with the same sampling rate, bit depth, and number of channels as the original Freesound uploads.

### Meta-Data Files

- **UrbanSound8k.csv:** A CSV file containing metadata information about each audio excerpt. The columns include:

  - **slice_file_name:**
    The name of the audio file in the format [fsID]-[classID]-[occurrenceID]-[sliceID].wav.

  - **fsID:**
    The Freesound ID of the recording from which the excerpt is taken.

  - **start:**
    The start time of the slice in the original Freesound recording.

  - **end:**
    The end time of the slice in the original Freesound recording.

  - **salience:**
    A subjective salience rating of the sound (1 = foreground, 2 = background).

  - **fold:**
    The fold number (1-10) to which the file has been allocated.

  - **classID:**
    A numeric identifier of the sound class (0-9).

  - **class:**
    The class name corresponding to the numeric identifier.

