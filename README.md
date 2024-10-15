# 👁️ Visual Assist Pose Guide

🦮 An assistive technology project that uses pose detection to guide visually impaired individuals through audio feedback.

## 📝 Description

This project leverages computer vision and pose detection to create an assistive system for visually impaired people. By using a camera to detect the movements of a sighted guide, the system provides audio cues to help a visually impaired person navigate their environment safely.

## ✨ Features

- 🎥 Real-time pose detection of a sighted guide using MediaPipe
- 🔊 Audio feedback system for direction and movement guidance
- 🎛️ Customizable audio cues for different movements and directions
- 🖥️ Easy-to-use interface for both the guide and the visually impaired user

## 🛠️ Requirements

- Python 3.7+
- OpenCV
- MediaPipe
- PyAudio (for audio output)
- NumPy
- Matplotlib (for development and debugging visualizations)

## 🚀 Installation

1. Clone this repository:
   ```
   git clone https://github.com/yourusername/visual-assist-pose-guide.git
   ```
2. Install the required packages:
   ```
   pip install opencv-python mediapipe pyaudio numpy matplotlib
   ```

## 🏃‍♂️ Usage

1. Run the main script:
   ```
   python visual_assist_guide.py
   ```
2. Position the camera to capture the sighted guide's full body
3. The sighted guide can perform the following actions:
   - 🚶‍♂️ Walk forward/backward
   - 🔄 Turn left/right
   - 🛑 Stop
   - ⚠️ Indicate obstacles or steps
4. The system will provide audio cues to the visually impaired person based on the guide's movements

## ⚙️ How it Works

The system uses MediaPipe to detect key points on the guide's body. It then interprets the position and movement of these points to determine the guide's actions:

- 📏 The vertical movement of the body indicates forward/backward motion
- 🔄 The rotation of the shoulders indicates turning
- 💪 Specific arm gestures can indicate stops, obstacles, or other important information

These interpretations are then translated into audio cues that instruct the visually impaired person on how to move.

## 🔧 Customization

You can adjust the sensitivity of movement detection and customize the audio cues in the `interpret_pose` and `generate_audio_cue` functions to suit different users' needs and preferences.

## ⚠️ Safety Considerations

This system is designed as an assistive tool and should not replace other mobility aids or techniques. Users should always prioritize their safety and use this system in conjunction with traditional mobility methods.

## 🤝 Contributing

Contributions, issues, and feature requests are welcome. Feel free to check the [issues page](https://github.com/SrivardhanS/Smart_glass_for_visually_impaired/issues) if you want to contribute.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [MediaPipe](https://mediapipe.dev/) for the pose detection solution
- [OpenCV](https://opencv.org/) for image processing capabilities
- The visually impaired community for inspiration and feedback

## 🔮 Future Improvements

- 🧠 Implement machine learning to improve accuracy of movement interpretation
- 📱 Develop a mobile app version for increased portability
- 🔗 Integrate with other assistive technologies for a more comprehensive solution
