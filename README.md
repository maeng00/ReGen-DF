# ReGen-DF: Reenactment & Generation DeepFake Face Dataset 

ReGen-DF is a **hybrid deepfake face dataset** that combines:

- **Text-to-Image (T2I) generated faces** from five modern generative models  
  (e.g., *seedream, kling, wan,* and other diffusion-based T2I models), and  
- **Face reenactment–based forgeries** built on top of **FFHQ real face images** using an AILab platform.

The goal of ReGen-DF is to provide a realistic and diverse benchmark for **deepfake detection**, **face forgery analysis**, and **robustness evaluation** under multiple generation pipelines.

---

## Dataset Download

The dataset is publicly available via Google Drive:

> 🔗 **Download ReGen-DF**  
> [ReGen-DF on Google Drive](https://drive.google.com/drive/folders/1dpZYkQhzo6AGMoIaWacV1AisBAa536_N?usp=drive_link)

> **Note:** Please make sure to read the *License & Usage* and *Ethical Considerations* sections before using the dataset.

---

## Key Characteristics

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

## License & Usage

The ReGen-DF dataset is released under the  
**Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0)** license.

- You **may** use, share, and adapt the dataset **for non-commercial research purposes only**.
- You **must** provide appropriate credit to the authors.
- If you create derivatives or adapted versions of this dataset, you **must distribute them under the same license** (CC BY-NC-SA 4.0 or a compatible license).
- Any **commercial use is not permitted** without explicit permission from the authors.

-> For the full legal text, please refer to **`license.txt`** in this repository  
and the Creative Commons page:  
https://creativecommons.org/licenses/by-nc-sa/4.0/

---

## Dataset Structure

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
```

---

## Sample Images

| Type            | Sample |
|-----------------|---------------------|
| T2I - seedream  | <img src="assets/samples/seedream_face_example.png" width="250"/> |
| T2I - kling     | <img src="assets/samples/kling_face_example.png" width="250"/>    |
| T2I - wan       | <img src="assets/samples/wan_face_example.png" width="250"/>      |
| T2I - flux       | <img src="assets/samples/flux_face_example.jpg" width="250"/>      |
| T2I - imagen       | <img src="assets/samples/imagen_face_example.jpg" width="200"/>      |
| T2V (basic) - kling       | <img src="assets/samples/kling_video_example.gif" width="250"/>      |
| T2V (lipsync) - kling       | <img src="assets/samples/kling_video_lipsync_example.gif" width="250"/>      |
| Face Reenactment    | <img src="assets/samples/emotions_happy.png" width="150"/> <img src="assets/samples/emotions_sad.png" width="150"/>  |

---

## Citation

If you use **ReGen-DF** in your research or project, please cite it as follows:

```bibtex
@dataset{regen_df_2025,
  title        = {ReGen-DF: Reenactment & Generation DeepFake Face Dataset},
  author       = {Jinseok Kim, Uihyeon Maeng, Heejung Jang, Suyeon Myeong},
  year         = {2025},
  howpublished = {GitHub and Google Drive},
  note         = {Available at \url{https://github.com/maeng00/ReGen-DF}}
}
