This repository provides some listening examples:

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

## 🏷️ Processing Method Description

The filenames indicate the processing method applied to each sample:

- **Original_Speech** – Clean speech signal at the error microphone
- **Unprocessed** – No active noise control (ANC) is applied
- **Ideal_KSANC** – ANC using the pure noise signal as the reference, representing a theoretical upper performance bound that is not realizable in practice   
- **Conventional_ANC** – ANC using the original noisy reference signal
- **DeepANC** – The method in “Deep ANC: A deep learning approach to active noise control”
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
