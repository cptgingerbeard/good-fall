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

## Use Case Scenarios

### Scenario 1: First-Time User Assessment
**Actor:** Elderly User (65+)  
**Goal:** Learn correct falling techniques

1. User uploads a fall training video.
2. System detects joints and movements.
3. System analyzes fall technique.
4. System provides detailed feedback and suggestions.
5. System tracks user progress over time.

### Scenario 2: Professional Rehabilitation Training
**Actor:** Physiotherapist  
**Goal:** Monitor patient fall prevention training

1. Therapist uploads patient training videos.
2. System analyzes movements and generates a detailed report:
   - Joint angle variations
   - Movement speed
   - Risk points
3. Therapist receives actionable insights for training.

### Scenario 3: Automatic Fall Technique Scoring
**Actor:** Automated System  
**Goal:** Evaluate fall training technique

1. Receive fall video input.
2. Identify 3D body position.
3. Calculate angles, speed, and acceleration.
4. Compare with ideal model.
5. Output numerical score and visual feedback.

### Technical Use Case: ML Model Training
**Actor:** System Administrator  
**Goal:** Improve fall detection algorithm

1. Collect fall training videos.
2. Annotate key movements.
3. Train machine learning model.
4. Validate accuracy.
5. Update fall detection system.


---

## Project Limitations

- Partial functionality: Detects falling vs. standing but not fall correctness.
- Requires video preprocessing: relevant frames must be extracted manually.
- Only detects the **leftmost** person in multi-person videos.
- Backend-only system; no frontend developed.
- Operates within Colab Notebook environment.

---

## What We Learned

- Improved proficiency in **Colab Notebook** and **Python**.
- Gained deeper understanding of **computer vision** and **machine learning**.
- Strengthened **team collaboration**, ensuring each member understood and contributed to the project.

---

## Future Directions

- Develop full fall classification system ("good" vs. "bad" falls).
- Implement a **frontend interface**.
- Refine fall detection algorithms for higher accuracy.

---
