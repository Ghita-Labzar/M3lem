# M3LEM – Digital Twin of Moroccan Artisans 

## Project Overview

**M3LEM** is an academic project aimed at preserving and transmitting **Moroccan cultural heritage**, specifically **Fassi embroidery (Terz Lfassi)**, through a **digital twin of an artisan**.

The project was motivated by a **growing lack of pupils and apprentices** willing or able to learn traditional embroidery, particularly **complex techniques such as Fassi brocade (Brocard)**. As master artisans age and fewer learners replace them, this know-how is increasingly at risk of being lost.

M3LEM proposes a **digital, immersive learning alternative**, combining **computer vision, deep learning, and 3D technologies** to capture, reproduce, and teach these gestures using a virtual human.

---

## Objectives

* Preserve traditional Moroccan craftsmanship digitally 🇲🇦
* Address the **decline in apprentices and pupils** learning traditional embroidery
* Safeguard complex techniques, especially **Fassi brocade (Brocard)**, which are at risk of disappearing
* Model and understand **artisan hand gestures** from real-world data
* Create an **educational digital twin** for learning and demonstration
* Avoid hardware dependency by using **video-based data**

---

## Data Collection

* **Source**: Public YouTube videos of **Terz Lfassi artisans**
* Videos were:

  * Selected for clarity and gesture visibility
  * Segmented into frames
  * Used to observe embroidery hand movements

⚠️ *Data was used strictly for academic and research purposes.*

---

## AI Model – CNN + LSTM (Python)

### Why CNN-LSTM?

Embroidery gestures are both:

* **Spatial** (hand position, needle orientation)
* **Temporal** (gesture sequences over time)

### Model Architecture

* **CNN**:

  * Extracts spatial features from each video frame
* **LSTM**:

  * Models temporal dependencies between consecutive gestures

### Pipeline

1. Video frame extraction
2. Feature extraction using CNN
3. Temporal modeling using LSTM
4. Output: embroidery gesture sequences

---

## 3D Processing – Blender

Blender was used as a critical intermediate step between AI and visualization:

* Rigging and skeleton alignment
* Hand and arm animation creation
* Mapping CNN-LSTM outputs to animations
* Exporting animations in **FBX format**

---

## Digital Twin – Unreal Engine + MetaHuman

* **MetaHuman** used to represent the artisan
* Blender animations imported into **Unreal Engine**
* Realistic reproduction of embroidery gestures
* Result: an interactive **digital twin for learning and visualization**
  
---

## Technologies Used

* **Python** – Data processing & deep learning
* **CNN + LSTM** – Gesture recognition
* **Blender** – 3D rigging & animation
* **Unreal Engine** – Real-time visualization
* **MetaHuman** – Digital human creation

---

## Key Contributions

* Cultural heritage preservation through technology
* Video-based gesture learning (no hardware required)
* Integration of AI with 3D animation pipelines
* High-quality visualization using MetaHuman

---

## Future Improvements

*Integrate the model in the MetaHuman
* Automated pose estimation from videos
* Larger and more diverse embroidery dataset
* Real-time interaction in Unreal Engine
* Extension to other Moroccan crafts


---

## License

This project is based on an original academic idea and implementation developed by the authors.

The concept, methodology, and integration pipeline are original work.

This repository is shared for educational and demonstration purposes only.

Unauthorized copying, reuse, or commercial exploitation of the idea, code, or content without explicit permission from the authors is not permitted.

© 2025 — All rights reserved.
