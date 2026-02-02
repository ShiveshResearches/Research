## Experiment: Effect of Environmental and Hardware Factors on Speech Recognition

| Experiment ID | Environment        | Microphone Used        | Internet Quality | Speaking Pace | Attempts | Successful Detection | Misinterpretation | Key Observation |
|--------------|--------------------|------------------------|------------------|---------------|----------|----------------------|-------------------|-----------------|
| E1           | Noisy room         | Laptop built-in mic    | Stable           | Normal        | 5        | 2                    | 2                 | High failure rate due to background noise and poor mic quality |
| E2           | Noisy room         | Bluetooth headset      | Stable           | Normal        | 5        | 5                    | 2                 | External mic improved detection, but recognition errors remained |
| E3           | Quiet + noisy mix  | Bluetooth headset      | Stable           | Fast          | Multiple | Reduced              | Increased         | Fast speech increased misinterpretation |
| E4           | Quiet environment  | Bluetooth headset      | Poor             | Normal        | Multiple | Inconsistent         | Increased         | Poor internet caused delays and incorrect recognition |
| E5           | Quiet environment  | Bluetooth headset      | Stable           | Slow & clear  | Multiple | High                 | Low               | Slow, clear speech improved accuracy significantly |

### Analysis
The experiments indicate that speech recognition accuracy is influenced more by environmental and external factors than by code logic. Background noise and microphone quality primarily affect detection, while speaking pace and internet stability impact recognition accuracy. These results suggest that improving input quality and system conditions can significantly enhance performance without modifying the core algorithm.

# A Comparative Study of Offline Speech Recognition Engines: CMU Sphinx vs Vosk

## Abstract
Speech recognition plays a critical role in modern human–computer interaction. While cloud-based solutions dominate the industry, offline speech recognition systems remain essential for privacy-sensitive, low-latency, and low-connectivity environments.  
This paper presents a comparative study of two offline speech recognition engines — **CMU Sphinx** and **Vosk**. The study evaluates their architecture, accuracy, usability, and real-world applicability. The results highlight the transition from traditional Hidden Markov Model (HMM)-based systems to modern deep-learning-based approaches.

---

## Keywords
Speech Recognition, Offline ASR, CMU Sphinx, Vosk, Kaldi, Deep Learning

---

## 1. Introduction
Automatic Speech Recognition (ASR) enables machines to interpret and transcribe human speech into text. Early ASR systems relied on statistical models such as Hidden Markov Models, while modern systems leverage deep neural networks for improved accuracy and robustness.

Offline speech recognition remains relevant due to:
- Privacy preservation
- Reduced latency
- Independence from internet connectivity

This paper compares **CMU Sphinx**, a classical ASR engine, with **Vosk**, a modern Kaldi-based engine, to analyze their effectiveness for contemporary applications.

---

## 2. Background

### 2.1 CMU Sphinx
CMU Sphinx is one of the earliest open-source speech recognition systems. It is based on Hidden Markov Models and Gaussian Mixture Models. While lightweight, its accuracy and adaptability are limited by outdated modeling techniques.

### 2.2 Vosk
Vosk is a modern offline speech recognition toolkit built on the Kaldi framework. It uses deep neural networks and supports multiple languages, accents, and real-time recognition.

---

## 3. Methodology

### 3.1 Experimental Setup
- Programming Language: Python  
- Execution Mode: Offline  
- Audio Input: Pre-recorded WAV files  
- Evaluation Environment: Local system  

### 3.2 Implementation Steps
1. Installation of CMU Sphinx and Vosk libraries.
2. Download and configuration of required acoustic and language models.
3. Processing identical audio samples through both engines.
4. Collection of transcription outputs.
5. Performance comparison based on defined metrics.

### 3.3 Evaluation Metrics
- Transcription accuracy
- Noise handling
- Real-time performance
- Ease of setup
- Language and accent support
- Development activity and community support

---

## 4. Comparative Analysis

| Feature / Aspect        | CMU Sphinx                  | Vosk                          |
|------------------------|-----------------------------|-------------------------------|
| ASR Architecture       | HMM + GMM                   | DNN (Kaldi-based)             |
| Offline Capability     | Yes                         | Yes                           |
| Accuracy               | Low–Medium                  | High                          |
| Noise Robustness       | Poor                        | Good                          |
| Real-time Processing   | Limited                     | Supported                     |
| Language Support       | Limited                     | Multiple languages            |
| Accent Handling        | Weak                        | Strong                        |
| Ease of Integration    | Difficult                   | Easy                          |
| Active Development     | Mostly inactive             | Actively maintained           |

---

## 5. Results and Discussion
The experimental results indicate that CMU Sphinx performs adequately only in controlled, noise-free environments. Its limited accuracy and outdated architecture restrict its usability in real-world applications.

Vosk demonstrated significantly higher accuracy, better noise handling, and smoother real-time recognition. Its active development and support for modern neural architectures make it suitable for contemporary AI systems.

---

## 6. Conclusion
This study highlights the technological evolution of offline speech recognition systems. While CMU Sphinx remains valuable for educational and historical understanding of ASR, it is not suitable for modern deployment.

Vosk outperforms CMU Sphinx across all evaluated parameters and is recommended for real-world offline speech recognition applications, especially in privacy-sensitive and low-resource scenarios.

---

## 7. Future Work
Future research may include:
- Benchmarking on low-end hardware
- Integration with live microphone input
- Comparison with cloud-based ASR systems
- Hybrid offline–online recognition models

---

## References
1. CMU Sphinx Documentation  
2. Vosk Speech Recognition Toolkit  
3. Kaldi ASR Framework

