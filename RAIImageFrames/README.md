# RAI Dataset Frame Images and Label Files Description

This directory contains frame images extracted from the RAI dataset videos, along with their corresponding label files. Each image represents a continuous 5-minute segment of the video. The frame images are arranged in chronological order and annotated with key frames (start and end of shots) from the label files, facilitating the analysis and observation of the video's structure and content.

## Directory Structure

This project contains two main folders, used to store the original dataset and the processed dataset:

- **RAIImageFrames/**
  - **original_dataset/**: Contains the original video frame images extracted from the RAI dataset along with their corresponding label files.
  - **processed_dataset/**: Contains the original video frame images extracted from the manually verified RAI dataset along with their corresponding label files.

## Frame Structure

- **Each frame image represents 5 minutes of video**: The frame images display video frames arranged one row per second, covering the duration of the 5-minute segment.
- **Key frame annotations**:
  - **Shot start frame**: Marked with a red rectangle, displaying the frame number.
  - **Shot end frame**: Marked with a green rectangle, displaying both the frame number and the shot index.

## Frame Naming Convention

Frame images are named sequentially in the following format:

    RAI-<video_number>-X.png

Where:
- `<video_number>` represents the video number, for example, `1` stands for video `1`.
- `X` is the frame image index. One image is generated every 5 minutes, starting from `1`. For example:
  - `RAI-1-1.png` represents the first 5 minutes of video `1`.
  - `RAI-1-2.png` represents the 5 to 10 minutes of video `1`.

Each RAI video corresponds to a `RAI-<video_number>.txt` file that contains shot labels, recording the start and end frames of each shot.

## Frame Image Source

These frame images are extracted from videos in the RAI dataset. The RAI dataset is available from the following website:

[Scene detection in Broadcast Videos - Imagelab, University of Modena and Reggio Emilia](http://imagelab.ing.unimore.it/imagelab/researchActivity.asp?idActivity=19)

## Notes

The frames are generated according to the actual frame rate and shot information of the video. To analyze specific content, please refer to the frame numbers and shot indices.
