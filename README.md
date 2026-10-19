# AI-PreFall-Risk-Detection

## About the Project
Falls can have serious consequences for older adults and people recovering from a stroke. Changes in posture, gait, and movement stability may provide useful information about a person's risk of falling.
This project explores the use of artificial intelligence and computer vision to identify movement patterns that may indicate a potential pre-fall condition. It uses camera-based human pose estimation to analyze body movements and generate warnings when the model detects patterns associated with increased fall risk.
The project also includes a caregiver dashboard that displays recorded alert events, helping make the system's output easier to monitor

## Problem Statement
Conventional observation may not always identify changes in movement early enough to support timely intervention. This project aims to develop a camera-based system that analyzes human movement, identifies potential pre-fall patterns, and communicates warnings through a caregiver monitoring interface.

## How It Works

The system follows a sequence of steps:

1. Camera input: Captures a person's movement in real time.
2. Human pose estimation: Uses MediaPipe to identify body landmarks from video frames.
3. Movement analysis: Extracts pose and movement features over time.
4. AI-based prediction: Processes a sequence of movement features using a trained machine learning model.
5. Warning generation: Produces a pre-fall risk warning when the model output meets the configured detection criteria.
6. Caregiver monitoring: Records alert events and makes them available through a web-based dashboard.

## Key Features

- Real-time, camera-based human movement analysis.
- Human pose estimation using MediaPipe.
- Temporal analysis of body pose and movement features.
- AI-based pre-fall risk prediction.
- On-screen warning and audible alert functionality.
- Caregiver dashboard for viewing recorded alert events.
- Testing with recorded videos and real-time camera input.

## Project Screenshots

 Real-Time-Pre-Fall-Detection.png

 Caregiver-Alert-Dashboard.png

## Technologies Used

- Programming language: Python
- Computer vision: OpenCV
- Pose estimation: MediaPipe
- Machine learning: TensorFlow / Keras
- Dashboard: HTML, CSS and JavaScript
- Data communication: Python-based HTTP server and API endpoints

## Model Evaluation

The trained pre-fall model was evaluated on a held-out test set.

Evaluation metric| Result
Test accuracy| 99.74%
ROC-AUC| 0.937
Precision–Recall AUC| 0.415
Test windows| 14,455
The test set contained 14,420 normal windows and 35 pre-fall windows. Because the classes are highly imbalanced, accuracy alone does not provide a complete picture of model performance. The precision–recall result and the number of correctly detected pre-fall cases must also be considered.
These results describe model performance on the current test set. They do not establish real-world clinical performance.

## Current Development Status
The project includes a trained pre-fall detection model, real-time camera testing, warning generation, and a caregiver dashboard for recorded alert events.
Further testing and refinement are needed to assess performance across different people, movement patterns, environments, and camera positions.

## Limitations
- Performance may vary with camera angle, lighting, visibility, and individual movement patterns.
- False alarms and missed warnings remain possible.
- Performance on a test dataset does not guarantee the same performance in real-world settings.
- The system is an academic assistive-monitoring prototype and is not a substitute for clinical assessment or a certified medical device.

## Future Improvements
- Evaluate the system with more diverse subjects and real-world movement conditions.
- Reduce false alarms while maintaining useful warning lead time.
- Improve caregiver notification and event-history features.
- Conduct further testing to assess reliability across different environments.

## Intended Application
The project explores how computer vision and artificial intelligence may support movement monitoring and caregiver awareness. Its purpose is to assist research into early movement-related warning patterns, not to guarantee fall prevention.

## Project Type
Academic project | Biomedical Engineering | Artificial Intelligence | Healthcare Technology
