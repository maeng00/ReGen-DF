# ReGen-DF: Reenactment & Generation DeepFake Face Dataset

ReGen-DF is a **hybrid deepfake face dataset** that combines:

- **Text-to-Image (T2I) generated faces** from five modern generative models  
  (e.g., *seedream, kling, wan,* and other diffusion-based T2I models), and  
- **Face reenactment–based forgeries** built on top of **FFHQ real face images** using an AILab platform.

The goal of ReGen-DF is to provide a realistic and diverse benchmark for **deepfake detection**, **face forgery analysis**, and **robustness evaluation** under multiple generation pipelines.

---

## 📦 Dataset Download

The dataset is publicly available via Google Drive:

> 🔗 **Download ReGen-DF**  
> [ReGen-DF on Google Drive](https://drive.google.com/drive/folders/1dpZYkQhzo6AGMoIaWacV1AisBAa536_N?usp=drive_link)

> **Note:** Please make sure to read the *License & Usage* and *Ethical Considerations* sections before using the dataset.

---

## 🔍 Key Characteristics

- **Hybrid Generation Pipelines**
  - **T2I-generated faces** from multiple state-of-the-art models  
    (e.g., seedream, kling, wan, and two additional diffusion-based generators).
  - **Reenacted faces** using FFHQ real identities and face reenactment techniques (via AILab platform).

- **Multiple Forgery Types**
  - Purely synthetic faces (no real image counterpart).
  - Identity-preserving reenactment forgeries based on real FFHQ faces.

- **Benchmark-Oriented Design**
  - Suitable for **binary deepfake detection** (real vs fake).
  - Can be extended to **source attribution** (which generator produced the fake).
  - Designed with **research reproducibility** in mind.

---

## 📁 Dataset Structure

The dataset is organized as follows (example structure):

```text
ReGen-DF/
├─ Genearaion/
│  ├─ seedream (5000)/
│  │  ├─ image_00000_sd.png
│  │  ├─ image_00001_sd.png
│  │  └─ ...
│  ├─ flux_output (979)/
│  ├─ imagen04_output (381)/
│  └─ ...
└─ Face Reenactment/
   ├─ output_emotions (155)/
   ├─ output_emotions_15000 (1480)/
   ├─ output_emotions_16000 (1481)/ 
   └─ ...

