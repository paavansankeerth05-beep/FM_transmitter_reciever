# 🎙 FM Transmitter and Receiver Project

## 📘 Overview
This project demonstrates the design and implementation of a low-power FM transmitter and receiver using basic analog components.  
The FM transmitter modulates an audio signal (from a microphone or line input) onto a high-frequency carrier wave, while the receiver demodulates the signal back into audio.  
Both circuits use a 2N3904 NPN transistor for amplification and oscillation.

---

## ⚡️ Objectives
- Design and construct an FM transmitter capable of broadcasting an audio signal.
- Build an FM receiver that can capture and reproduce the transmitted signal.
- Understand the principles of frequency modulation (FM), oscillator circuits, and RF communication.

---

## 🧩 Components Used

### Common Components
| Component | Specification | Quantity |
|------------|----------------|-----------|
| 2N3904 | NPN Transistor | 2 |
| Capacitors | 5 pF – 47 µF | Various |
| Resistors | 470 Ω – 27 kΩ | Various |
| Inductor | 1 µH – 10 µH | 2 |
| Battery | 9V or 12V | 1 each |
| Antenna | 10–20 cm wire | 2 |
| Audio Source / Mic | Electret microphone or mono input | 1 |

---

## 📡 Transmitter Circuit

### 🧠 Working Principle
The transmitter uses the 2N3904 transistor configured as a Colpitts oscillator, generating an RF carrier frequency in the 88–108 MHz FM band.  
An audio input signal modulates the base bias voltage, causing small variations in the oscillator frequency — achieving frequency modulation (FM).

### ⚙️ Circuit Description
- C1, R1, C2 form the audio coupling network.
- R2, L1, C3, and C4 create the oscillator tank circuit.
- Q1 (2N3904) acts as both an amplifier and oscillator.
- C5 couples the RF signal to the antenna for transmission.

### 🔧 Transmitter Specifications
| Parameter | Value |
|------------|--------|
| Supply Voltage | 9V |
| Frequency Range | 88 MHz – 108 MHz |
| Output Power | <10 mW |
| Modulation Type | Frequency Modulation (FM) |
| Audio Input | 3.5 mm mono or microphone |

---

## 📻 Receiver Circuit

### 🧠 Working Principle
The receiver is a basic single-transistor FM detector.  
It uses a tuned LC tank circuit to pick up the transmitted FM signal.  
The 2N3904 transistor amplifies and demodulates the signal, and the output can be fed to an amplifier or headphones.

### ⚙️ Circuit Description
- Electret Microphone captures audio signals for transmission.
- Inductor (1 µH) and capacitors (39 pF, 1 nF, 5 pF) determine the resonance frequency.
- Q1 (2N3904) serves as the RF amplifier and detector.
- Output can be connected to a small speaker or earphone.

### 🔧 Receiver Specifications
| Parameter | Value |
|------------|--------|
| Supply Voltage | 9V – 12V |
| Frequency Range | Tuned to 88–108 MHz |
| Output | Audio signal (demodulated FM) |
| Sensitivity | ~1 µV for clear reception |

---

## 🧠 Theory of Operation

### Frequency Modulation (FM)
In FM, the frequency of the carrier wave changes according to the amplitude of the input (audio) signal, while the amplitude remains constant.  
This makes FM more resistant to noise compared to AM.

### Oscillator Design
Both circuits rely on an LC tank circuit, consisting of an inductor (L) and capacitor (C).  
The oscillation frequency is given by:
\[
f = \frac{1}{2\pi\sqrt{LC}}
\]
By adjusting the capacitance or inductance, the circuit can be tuned to a specific FM frequency band.

---

## 🧪 Simulation and Testing
You can simulate the transmitter and receiver circuits using:
- Multisim
- LTSpice
- Proteus
- Falstad Circuit Simulator

### Steps:
1. Connect the transmitter output antenna.
2. Tune the receiver LC circuit until you get a clear audio signal.
3. Adjust the antenna length and capacitor values for better range and clarity.

---

## 🧰 Applications
- Wireless audio transmission (short range)
- Educational demonstrations of RF and FM principles
- Small-scale communication experiments
- Wireless microphone or spy transmitter prototype

---
## 🧠 Key Learnings
- Basics of RF oscillation and modulation
- Design of Colpitts oscillators
- Understanding LC tank circuits
- Practical issues in RF tuning and noise reduction

---

## 🪛 Troubleshooting Tips
| Problem | Possible Cause | Solution |
|----------|----------------|-----------|
| No transmission | Power or connection issue | Check battery and transistor orientation |
| Distorted audio | Improper biasing | Adjust R1 and R2 values |
| Short range | Antenna too short or frequency mismatch | Increase antenna length, tune L and C |
| No reception | Out of tuning range | Adjust tuning capacitor or coil turns |

---

## 📸 Circuit Diagrams
Transmitter Circuit:
<img width="872" height="514" alt="image" src="https://github.com/user-attachments/assets/7dbbc944-2aa8-401a-8aa4-eee1dcf1a889" />


Receiver Circuit:
<img width="1280" height="677" alt="image" src="https://github.com/user-attachments/assets/f42e353b-ca69-4bf0-9765-a55c6cf87105" />

---

## 🧩 Future Enhancements
- Add stereo transmission capability
- Include digital frequency display
- Use PLL-based tuning for stability
- Integrate audio amplifier (LM386) for clearer sound output

---

## 👥 Contributors
This project was collaboratively designed and tested by:
- Paavan sankeerth

---

## 📬 Contact
For queries or collaboration:
Email:paavansankeerth05@gmail.com  
GitHub: https://github.com/paavansankeerth05-beep
