# good-fall
project "good-fall"


# Good Fall Project

**Submitted by:**  
Maor Ben David  
Yuval Hermon  
Carmela Falishtayev

---

## Executive Summary

The **Good Fall** project is a technological system designed to assist individuals aged 65 and older in learning how to fall correctly, thereby helping to prevent severe injuries. Leveraging advanced body movement recognition and computer vision, the system offers personalized feedback on fall performance—including graphical representations and stick-figure identification. It processes videos of fall training sessions, detects body positions, calculates angles and acceleration, and identifies the frame numbers where a fall is detected.

---

## Development Areas (Main Modules)

### Body Recognition
This module identifies all body joints to accurately detect the body and classify the fall as correct or incorrect. It enables precise recognition of movements for quick identification of falling techniques.

### Position and Transition Recognition
This module detects key user positions (e.g., standing, falling) and transitions between them. It reliably determines when a user is in a falling state.

---

## Technologies and Tools

The project utilizes several advanced tools and platforms:

- **Colab Notebook:** Used for development and testing. It supports professional Python execution for modeling and machine learning.
  
- **excercise_pose_classifier_ido_video1.ipynb:**  
  This notebook focuses on classifying body postures by detecting key body points and constructing a 3D posture representation from video frames.

### Key Functionalities

#### Body Posture Classification
Identifies major body points (head, hands, legs) and generates a 3D representation to determine the user's state (standing or falling).

#### Angle Calculation in 3D Space
Uses XYZ coordinates to calculate angles between body points, helping assess posture during movement.

#### Speed and Acceleration Calculation
Calculates speed and acceleration of body points across frames to distinguish between standing and falling movements.

---


## Future Directions

- Develop full fall classification system ("good" vs. "bad" falls).
- Implement a **frontend interface**.
- Refine fall detection algorithms for higher accuracy.

---
