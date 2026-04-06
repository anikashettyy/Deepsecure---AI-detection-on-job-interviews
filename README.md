# Deepsecure---AI-detection-on-job-interviews
DeepSecure is a prototype deepfake detection system that compares two video inputs to identify potential AI manipulation. It analyzes facial patterns and inconsistencies to generate a suspicion score. The system is designed to enhance authenticity in remote interviews and can be scaled using advanced deep learning for real-time deployment.

🔍 1. Real-Time Face Detection & Tracking

The system continuously detects and tracks the candidate’s face using OpenCV.
Ensures a human face is always present in the frame
Detects multiple faces (possible malpractice)
Flags cases where the face disappears or is partially hidden

This prevents impersonation and ensures only one candidate is present.

👁️ 2. Blink Detection (Liveness Check)

DeepSecure uses eye aspect ratio (EAR) calculations to monitor blinking patterns.

Detects natural human blinking behavior
Identifies abnormal or no blinking, which may indicate deepfake or pre-recorded video

Helps distinguish between a real person and synthetic/generated faces.

🎭 3. Deepfake Behavior Analysis

The system analyzes subtle inconsistencies in facial movements and expressions:

Unnatural facial motion
Delayed or mismatched lip-sync
Irregular eye movement

These are common indicators of deepfake-generated content.

💡 4. Lighting & Background Monitoring

DeepSecure evaluates environmental conditions:

Detects sudden lighting changes (e.g., screen overlays)
Identifies bright backlight issues that affect detection accuracy
Flags suspicious background activity

Improves robustness and reduces false positives.

🔊 5. Audio Presence Detection

The system checks for audio signals during the session:

Ensures candidate is actively speaking when required
Detects absence of sound or unnatural silence

Helps verify active participation and detect pre-recorded responses.

⚠️ 6. Suspicious Activity Alerts

If any anomaly is detected, the system:

Generates real-time alerts
Logs suspicious events for later review
Can be extended to notify interviewers instantly

🖥️ 7. User Interface for Monitoring

Built with a GUI (Tkinter), the system provides:

Live webcam feed
Detection status indicators
Easy controls for starting/stopping monitoring

🎯 Overall Goal
DeepSecure aims to maintain fairness and integrity in online interviews by ensuring:

The candidate is real
The session is live
No deepfake or impersonation tools are being used
Use Cases
Online job interviews
Remote examinations
Virtual hiring platforms
Proctored assessments.
