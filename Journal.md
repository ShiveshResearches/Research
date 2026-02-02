# Research Journal – Voice-Controlled Systems

**Name:** Shivesh Pratap Singh  
**Project:** Research 1 — Speech Recognition Reliability in Voice-Controlled Systems

This journal documents my daily work, experiments, failures, assumptions, and learning
while developing and studying a Python-based voice-controlled automation system.
The goal is to capture **thinking and growth**, not just results.

---

## Entry 1 — Understanding Online Speech Recognition

**Date:** 2026-02-01  
**Time Spent:** ~1 hour  
**Research Phase:** Initial System Evaluation (Online ASR)

### Goal for the Day
To understand how the speech recognition component of my voice assistant works and to explore how the project could be framed as a **research study**, rather than just a functional application.

### What I Worked On
I carefully reviewed my existing Python code, focusing on the speech recognition function. I examined how audio input was processed and how text output was generated. I also studied the `recognize_google(audio)` method used from the `SpeechRecognition` library.

### Incorrect Assumption Identified
I initially assumed that speech recognition was being performed locally by my program.

After reviewing documentation and understanding the system flow, I realized that:
- The audio is sent to **Google’s servers**
- Speech-to-text processing is entirely **cloud-based**
- My system depends on internet connectivity and external infrastructure

### What I Learned
- Recognition failures are not always caused by bugs in code
- External factors such as:
  - background noise
  - microphone quality
  - speaking style
can significantly affect recognition accuracy

This was a major shift in how I understood the problem.

### Next Steps
Identify all system-level and environmental factors affecting recognition accuracy and design controlled experiments to test them.

---

## Entry 2 — Controlled Experiments on Online Speech Recognition

**Date:** 2026-02-02  
**Research Phase:** Experimental Evaluation (Online ASR)

### Experiment Objective
To determine whether speech recognition failures were due to:
- code-level issues  
or  
- external/environmental factors

Variables tested:
- Background noise
- Microphone quality
- Internet connectivity
- Speaking pace

---

### Experimental Setup

**Hardware**
- Budget laptop with built-in microphone
- Bluetooth headset with dedicated microphone

**Software**
- Python
- `SpeechRecognition` library
- Google Speech Recognition API (online)

**Environment**
- Noisy room
- Same physical environment used across all tests for consistency

---

### Experiments & Observations

#### Experiment E1: Built-in Laptop Microphone (Noisy Environment)
- Total attempts: 5  
- Speech not detected: 3  
- Speech detected but misinterpreted: 2  
- Correct recognitions: 0  

**Observation:**  
The system performed poorly in noisy conditions when using the laptop’s built-in microphone.

---

#### Experiment E2: Bluetooth Headset (Same Environment)
- Total attempts: 5  
- Speech detected: 5  
- Misinterpretations: 2  
- Correct recognitions: 3  

**Observation:**  
A better microphone significantly improved detection consistency, though accuracy was still imperfect.

---

#### Experiments E3–E5: Controlled Variations
Additional tests varied:
- Speaking speed (fast vs slow)
- Internet quality (stable vs unstable)

**Findings**
- Poor internet caused delays and incorrect recognition
- Fast speech increased misinterpretation
- Clear speech and stable internet improved accuracy significantly

---

### Key Learnings
Most recognition failures were caused by **external factors**, not faulty code:
- Background noise
- Microphone limitations
- Internet dependency

This corrected my earlier belief that recognition errors were primarily programming mistakes.

---

### Limitations Identified
- Strong dependency on internet connectivity
- Reduced performance in noisy environments
- Sensitivity to microphone quality and speech clarity

---

### Conclusion
Online speech recognition reliability depends more on **environmental and system constraints** than on the program logic itself. Understanding this reframed the project from debugging code to studying system behavior.

---

### Planned Next Step
Explore **offline speech recognition systems** to reduce internet dependency.

Planned tools:
- Vosk
- CMU Sphinx

---

## Entry 3 — Offline ASR Comparison & Research Documentation

**Date:** 2026-02-02  
**Research Phase:** Conceptual Expansion & Documentation

### Focus for the Day
Formalizing the research by:
- Comparing offline ASR systems
- Structuring the project as a proper research repository

### What I Worked On
Instead of writing new code, I focused on:
- Comparing **CMU Sphinx** and **Vosk**
- Writing a research-style comparative study (`Experiment.md`)
- Designing a clear and professional `README.md`

---

### Key Actions Taken
- Documented differences between:
  - Classical ASR (HMM-based CMU Sphinx)
  - Modern ASR (DNN-based Vosk)
- Compared:
  - Accuracy
  - Noise robustness
  - Ease of use
  - Real-world applicability
- Learned how to separate:
  - `README.md` → research intent & navigation
  - `Experiment.md` → experiments & analysis

---

### Important Realizations
- Research is not only about implementation — **documentation is part of research**
- CMU Sphinx is mainly useful for historical and educational understanding
- Vosk represents the current practical standard for offline ASR
- Repository structure itself reflects research maturity

---

### Constraints Faced
- No access to a device capable of running VS Code or testing ASR locally
- Shifted focus to:
  - conceptual understanding
  - system design
  - academic documentation

This reinforced that lack of resources does not stop research — it reshapes it.

---

### Reflection
This project is no longer just about building a voice assistant.

It is about:
- questioning assumptions
- understanding system limitations
- documenting intellectual growth honestly

This approach feels strongly aligned with the research culture I aim to be part of at **MIT**.

---
