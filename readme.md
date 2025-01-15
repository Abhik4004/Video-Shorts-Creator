## Video Frame Difference Detection (Python)

This repository contains Python code to identify frames with significant changes in a video. It achieves this by analyzing the absolute difference between consecutive frames.

### Description

The script processes a video file and removes frames that are very similar to the previous frame. This can be useful for tasks like:

- Creating highlight reels from videos
- Reducing video size by removing redundant frames
- Detecting scene changes

### Usage

1. **Clone the repository:**

   ```bash
   git clone https://github.com/Abhik4004/Video-Shorts-Creator.git
   ```

2. **Install dependencies:**

   This script requires OpenCV (cv2). Install it using:

   ```bash
   pip install opencv-python
   ```

   Replace `<video_path>` with the path to your video file.

3. **Output:**

   The script prints the number of frames identified as having significant changes and potentially writes these frames to a new video file (optional).

### Functionality

The script performs the following steps:

1. Opens the video using OpenCV.
2. Iterates through each frame.
3. Calculates the absolute difference between the current and previous frame.
4. Uses either a fixed threshold or Otsu's thresholding to identify frames with significant differences.
5. Optionally, saves these frames with significant changes to a new video file.

### Options

- **Threshold (optional):** By default, the script uses Otsu's thresholding to determine frame changes. You can modify the script to use a fixed threshold instead.
- **Output video (optional):** Currently, the script only prints the number of frames with changes. You can modify the script to save these frames to a new video file.

### Further Enhancements

- Explore more sophisticated methods for change detection like Structural Similarity Index (SSIM) for better handling of lighting changes.
- Implement background subtraction techniques if your video has a static background.
- Add options for adjusting the sensitivity of change detection.

### Contributing

Feel free to contribute to this project by:

- Reporting issues or bugs.
- Suggesting improvements to the code or documentation.
- Implementing new features or functionalities.

Please refer to the contributing guidelines (if available) before submitting pull requests.

### License

This project is licensed under [insert your preferred license here] (e.g., MIT License). See the LICENSE file for details.

# Video-Shorts-Creator
