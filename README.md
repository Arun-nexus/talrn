# Article-Based Image Generation Using Transformer Summaries & Stable Diffusion

This project demonstrates an end-to-end pipeline that converts long-form textual articles into high-quality AI-generated images using large language models and diffusion pipelines.  

The system:
1. Summarizes the article using a transformer-based abstractive summarizer  
2. Extracts meaningful keywords using spaCy  
3. Builds intelligent context-aware prompts  
4. Merges prompts with a custom style prompt  
5. Generates multiple images using two different diffusion models  
6. Saves and visualizes all images  
7. (Optional) Exports everything into a DOCX report

---

## Features

### ✔ Automated Text Processing  
- Abstractive summarization using **facebook/bart-large-cnn**  
- Keyword extraction using **spaCy noun chunks**  

### ✔ Smart Prompt Engineering  
- Dynamically built prompts from summary + keywords  
- Human-style custom prompt merging  
- Supports multiple prompt variants

### ✔ Dual Image Generation Models  
- **Stable Diffusion v1.5** (quality-focused)  
- **SD Turbo** (speed-focused)  
- Both used to generate 4 images each for comparison

### ✔ Modular & Clean Code  
- Each step is separated into functions  
- Can be easily replaced with any other summarizer or diffusion model

### ✔ Multiple Output Formats  
- Images saved under `./outputs/`  
- Visualized using Matplotlib  
- Option to generate a **DOCX report** with embedded images

---

##  Technologies Used

| Component | Library/Model |
|----------|----------------|
| Summarization | BART (facebook/bart-large-cnn) |
| Keyword Extraction | spaCy (en_core_web_sm) |
| Prompt Generation | Custom logic |
| Image Generation | Diffusers Pipeline (Stable Diffusion + SD Turbo) |
| Visualization | Matplotlib |
| Optional Report | python-docx |

---

## 📁 Project Structure

