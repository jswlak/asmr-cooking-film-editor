# 🎬 AI Scene Sound Enhancer  
### *Auto-detect cooking scenes like salt sprinkling or vegetable chopping, and overlay realistic ASMR sounds automatically.*

---

## 🧠 Overview
**AI Scene Sound Enhancer** is an intelligent film-editing tool that automatically detects fine-grained actions (like *salt sprinkling*, *vegetable chopping*, or *stirring*) in cooking or ASMR videos, and overlays matching sound effects to enhance the sensory experience.

This project combines **Computer Vision**, **Audio Processing**, and **AI-based scene understanding** — aiming to automate parts of the video editing process.

---

## 🎯 Core Features

✅ **Action Detection**
- Detects events such as:
  - 🧂 Salt Sprinkling  
  - 🔪 Vegetable Chopping  
  - 🥄 Stirring / Mixing  
- Uses pretrained video action recognition models for detection.

✅ **Sound Overlay**
- Automatically adds contextually relevant sound effects.
- Synchronizes based on detected event timestamps.
- Adjusts volume, fade-in/out, and mixing automatically.

✅ **Video Editing Pipeline**
- Input: Raw cooking/ASMR video  
- Output: Enhanced video with layered sounds  
- Fully automated using Python scripts.

✅ **Extendable**
- Add new actions easily by fine-tuning or mapping new sounds.  
- Scalable to emotional music overlay, ambient enhancement, or background scoring.

---

## 🧩 System Architecture

Video Input
↓
Frame/Clip Extraction
↓
Pretrained Action Detection Model (3D CNN / Video Transformer)
↓
Event Timeline (start_time, end_time, label)
↓
Sound Mapping (label → sound.mp3)
↓
Audio Overlay & Mixing (MoviePy / PyDub)
↓
Final Enhanced Video Output


---

## 🛠️ Tech Stack

| Category | Tools & Libraries |
|-----------|------------------|
| **Core Language** | Python 3.x |
| **Video Processing** | OpenCV, MoviePy, FFmpeg |
| **AI / ML Models** | PyTorch, Torchvision, PytorchVideo |
| **Pretrained Models** | Kinetics-400 / 700, ActionFormer, I3D, Video Swin Transformer |
| **Audio Tools** | PyDub, Librosa, Audiomentations |
| **Annotation (optional)** | Label Studio, CVAT |
| **UI (optional)** | Tkinter / PyQt / Gradio / Streamlit |

---

## 🚀 Getting Started

