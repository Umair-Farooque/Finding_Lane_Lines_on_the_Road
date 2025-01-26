# Finding Lane Lines on the Road

## Project Overview
This project involves detecting lane lines on the road using computer vision techniques. It is implemented in a Jupyter Notebook, leveraging Python libraries such as OpenCV, NumPy, and Matplotlib. The application is designed to process video or image frames captured from a vehicle's front-facing camera, identifying and highlighting lane markings to assist in safe navigation.

## Features
- **Image Preprocessing**: Converts input frames to grayscale, applies Gaussian blur, and detects edges using the Canny edge detection algorithm.
- **Region of Interest Selection**: Focuses on the road area where lane lines are expected.
- **Hough Transform Line Detection**: Detects lane lines using the Hough transform and overlays them on the original frame.
- **Video Processing**: Processes a sequence of frames from video input to create an annotated video output.

## Requirements
- Python 3.7 or later
- Jupyter Notebook

### Libraries
- OpenCV
- NumPy
- Matplotlib

To install the required libraries, use the following command:
```bash
pip install opencv-python-headless numpy matplotlib
```

## File Structure
1. **Finding_Lane_Lines_on_the_Road.ipynb**: The main project file containing the code and explanations.
2. **Test Images/Video**: Sample input files (not included in this repository) to demonstrate the lane detection functionality.
3. **Output**: Annotated images or videos showcasing the detected lane lines.

## How to Run
1. Open the `Finding_Lane_Lines_on_the_Road.ipynb` file in Jupyter Notebook.
2. Execute the cells sequentially to process the sample inputs.
3. Modify the input paths to use custom images or videos for testing.

## Key Functions
1. **Grayscale Conversion**: Simplifies the image data for processing.
2. **Edge Detection**: Identifies potential lane edges.
3. **Hough Transform**: Extracts line segments representing lane lines.
4. **Overlay**: Combines the detected lines with the original input.

## Sample Results
The implementation highlights lane lines in yellow (right lane) and white (left lane) for clarity. Annotated videos/images can be saved for further analysis.

## Customization
- Adjust the region of interest coordinates to suit different camera perspectives.
- Modify the Canny edge detection thresholds for specific lighting conditions.
- Tweak the Hough transform parameters to refine line detection.

## Known Issues
- Lane detection accuracy may reduce in poor lighting or adverse weather conditions.
- The algorithm may struggle with curved lanes or poorly marked roads.

## Future Improvements
- Support for curved lane detection using polynomial fitting.
- Integration with real-time video streams.
- Improved robustness under varying lighting and weather conditions.

## Credits
This project is inspired by basic computer vision principles and serves as an introductory application for detecting road features.

