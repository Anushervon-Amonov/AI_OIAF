AI_OIAF 🌱

AI Offline Intelligent Agriculture Farmer

AI OIAF is an offline-first Android AI system designed to help farmers identify plants and analyze plant conditions using photographs.

The project is designed especially for agricultural environments where internet access may be limited or unstable.

How It Works

📷 Photo
   ↓
🌱 Plant Filter
   ↓
Is it a plant?
   ├── No → 🚫 Stop analysis
   │
   └── Yes
        ↓
🔬 PV25 AI Model
        ↓
📋 Plant Classification
        ↓
💡 Agricultural Assistance

AI Pipeline

1. Plant Filter

The first AI model checks whether the submitted image contains a plant.

Plant → continue to the main AI model

Non-Plant → stop the analysis and ask the user to photograph a plant or leaf.

This prevents the main classification model from processing irrelevant images.

2. PV25

If a plant is detected, the image is passed to the PV25 model for further plant and condition classification.

The models run locally on the Android device using ONNX Runtime.

Key Features

- 📱 Android application
- 📴 Offline AI inference
- 🌱 Plant detection
- 🔬 Plant and condition classification
- ⚡ ONNX Runtime
- 📷 Image-based analysis
- 🌍 Designed for areas with limited or unstable internet access
- 🤖 Multi-stage AI pipeline

Technology

- Kotlin
- Android
- ONNX Runtime
- PyTorch
- TensorFlow
- MobileNetV3
- Computer Vision
- Deep Learning

AI Models

The current application uses two ONNX models.

Plant Filter

Detects whether an image contains a plant.

Classes:

- NonPlant
- Plant

PV25

Performs the main plant and condition classification.

Project Goal

The long-term goal of AI OIAF is to provide a practical, low-connectivity agricultural AI assistant that can help farmers make better decisions using only a smartphone.

The project is being developed with a focus on offline operation, real-world agricultural images, and accessibility in rural environments.

Developer

Anushervon Amonov

AI OIAF is an ongoing independent AI and agricultural technology project.
