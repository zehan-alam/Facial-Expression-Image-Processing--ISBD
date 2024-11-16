# Facial Expression Image Processing Project

This project presents a solution to a facial expression recognition challenge from Innovative Skills BD.

**Dataset Used**: [FER-2013 dataset](https://www.kaggle.com/datasets/msambare/fer2013)

### Project Tasks
This project involved addressing the following tasks:
1. **Image Quality Enhancement**: Improved image quality by applying brightness and contrast enhancement techniques.
2. **Facial Feature Segmentation**: Segmented key facial features, including eyes and mouth, for focused analysis.
3. **Edge Detection**: Applied edge detection to analyze facial structures and enhance expression clarity.
4. **Selective Blurring**: Blurred non-essential image areas to keep the focus on facial expressions.

### Approach
To evaluate the approach, I selected 10 random images from the dataset and performed the following steps:

- **Scaling**: Since the images are low resolution, I used the `cv2.INTER_CUBIC` interpolation method to upscale each image by 2x.
- **Color Enhancement**: Applied CLAHE (Contrast Limited Adaptive Histogram Equalization) to enhance color details.
- **Denoising**: Used `cv2.fastNlMeansDenoisingColored` to reduce noise, making facial features more distinct.
- **Edge Detection**: Applied Canny edge detection to emphasize facial contours and expressions.
- **Feature Detection**: Used `cv2.CascadeClassifier` to detect eyes, face, and mouth, helping isolate important facial components for analysis.

### Results
The processed outputs for all 10 selected images are included, showcasing the enhancements and feature segmentation applied. This project demonstrates techniques for improving facial expression visibility and focus, providing foundational steps toward more accurate emotion recognition in image data.
