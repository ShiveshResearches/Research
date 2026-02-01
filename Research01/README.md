# Research : Impact of Environmental Factors on Speech Recognition Accuracy

## Overview
This project explores how real-world factors such as background noise, microphone quality, speaking pace, and internet connectivity affect the accuracy of speech recognition systems.

The goal of this research was to determine whether recognition errors were caused by flaws in the code itself or by external environmental conditions.

This study was conducted through practical experiments using different audio input setups and environments.

---

## Motivation
Speech recognition systems are widely used in voice assistants and AI applications. While developing a basic speech recognition system, frequent misinterpretations were observed.

Instead of immediately assuming code-level issues, this research investigates **external variables** that influence recognition accuracy.

---

## Experimental Setup

### Hardware Used
- Budget laptop (built-in microphone)
- Bluetooth headset (external microphone)

### Environments Tested
- Noisy room
- Same noisy room with external microphone
- Stable internet connection
- Unstable internet connection

---

## Experiments Conducted

### Experiment 1: Noisy Environment with Built-in Microphone
- Environment: Noisy room
- Microphone: Laptop microphone
- Attempts: 5

**Results**
- Command not detected: 3 times
- Command detected but misunderstood: 2 times

**Inference**
- Background noise significantly affects detection.
- Built-in microphones are unreliable in noisy environments.

---

### Experiment 2: Noisy Environment with Bluetooth Headset
- Environment: Same noisy room
- Microphone: Bluetooth headset
- Attempts: 5

**Results**
- Command detected successfully: 5 times
- Misinterpretation: 2 times

**Inference**
- External microphones improve detection accuracy.
- Recognition errors still occur due to other factors.

---

### Experiment 3: Speaking Pace and Internet Connectivity
Additional tests were conducted by varying:
- Speaking speed (fast vs slow)
- Internet quality (good vs poor)

**Observations**
- Fast speech increased misinterpretation.
- Poor internet connection caused delayed or incorrect recognition.
- Slow, clear speech improved accuracy.

---

## Key Findings

Speech recognition accuracy is negatively affected by:
- Background noise
- Poor microphone quality
- Unstable internet connection
- Fast or unclear speech

Most recognition issues were **not caused by the code**, but by external conditions.

---

## Conclusion
This research demonstrates that environmental and hardware factors play a crucial role in speech recognition performance. Improving microphone quality, ensuring stable internet connectivity, and minimizing background noise can significantly enhance system accuracy.

These findings emphasize the importance of testing AI systems in real-world conditions rather than ideal environments.

---

## Future Improvements
- Noise cancellation preprocessing
- Offline speech recognition testing
- Dataset-based accuracy evaluation
- Testing with different accents and languages

---

## Author
Shivesh Pratap Singh

## License
This project is open for educational and research purposes.
