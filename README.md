# Reference Signal Enhancement for KSANC

This repository provides some listening examples.

---

## 🎧 Listening Comparison

### Sample 00606 – Fan Noise – SNR −5 dB

| Method | Audio |
|--------|-------|
| Original Speech | <audio controls><source src="./Test_samples/SNR_-5dB/fan/00606_Original_Speech.wav" type="audio/wav"></audio> |
| Unprocessed | <audio controls><source src="./Test_samples/SNR_-5dB/fan/00606_Unprocessed.wav" type="audio/wav"></audio> |
| Ideal KSANC | <audio controls><source src="./Test_samples/SNR_-5dB/fan/00606_Ideal_KSANC.wav" type="audio/wav"></audio> |
| Conventional ANC | <audio controls><source src="./Test_samples/SNR_-5dB/fan/00606_Conventional_ANC.wav" type="audio/wav"></audio> |
| DeepANC | <audio controls><source src="./Test_samples/SNR_-5dB/fan/00606_DeepANC.wav" type="audio/wav"></audio> |
| RSE-based KSANC | <audio controls><source src="./Test_samples/SNR_-5dB/fan/00606_RSE_KSANC.wav" type="audio/wav"></audio> |

---

## 🏷️ Processing Method Description

The filenames indicate the processing method applied to each sample:

- **Original_Speech** – Clean speech signal at the error microphone  
- **Unprocessed** – No ANC applied, containing both noise and speech 
- **Ideal_KSANC** – ANC using the pure noise reference (theoretical upper bound)
- **Conventional_ANC** – ANC using the original reference signal
- **DeepANC** – DeepANC baseline method  
- **RSE_KSANC** – Proposed reference signal enhancement method 

## 🔢 Filename Convention

Example:

00606_RSE_KSANC.wav

Where:

- `00606` → Sample index  
- `RSE_KSANC` → Processing method  

The repository includes listening examples for two randomly selected samples:

- **00173**
- **00606**

---

## 🎧 Listening Examples

Audio samples are organized by signal-to-noise ratio (SNR) and noise type.

### SNR Conditions
- **SNR −5 dB**
- **SNR 5 dB**

### Noise Types
- Fan  
- Engine  
- Gearbox  
- Bearing  

---

## 📂 Directory Structure

```
Test_samples
├── SNR_-5dB
│   ├── fan
│   │   ├── 00606_Original_Speech.wav
│   │   ├── 00606_Unprocessed.wav
│   │   ├── 00606_Ideal_KSANC.wav
│   │   ├── 00606_Conventional_ANC.wav
│   │   ├── 00606_DeepANC.wav
│   │   └── 00606_RSE_KSANC.wav
│   ├── engine
│   ├── gearbox
│   └── bearing
│
└── SNR_5dB
    ├── fan
    ├── engine
    ├── gearbox
    └── bearing
```
