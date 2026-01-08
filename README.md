# ✨ Magic Ad Generator

**AI Creative Assistant: Generate Ad Ideas & Visuals in One Click.**

[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://magicadsgenerator.streamlit.app/)


## 🚀 About The Project
Magic Ad Generator is a generative AI application designed to streamline the creative advertising workflow. It acts as a virtual agency, combining a **Creative Director (LLM)** and an **Art Director (Image Generation Model)** to produce ready-to-use ad assets instantly.

This project was built to demonstrate the practical application of **Large Language Models (LLM)** and **Stable Diffusion** in a real-world business context (AdTech).

## 🧠 How It Works
1.  **User Input:** Enters a product name and desired "vibe" (target audience).
2.  **AI Copywriter (Text):** The app sends a prompt to **Qwen 2.5-72B-Instruct**, instructing it to generate an engaging Instagram caption and a detailed English image prompt.
3.  **AI Illustrator (Visual):** The generated image prompt is seamlessly passed to **Stable Diffusion XL**, which renders a high-quality product visualization.
4.  **Result:** The user gets a complete ad package (Visual + Caption) in seconds.

## 🛠️ Tech Stack
* **Framework:** [Streamlit](https://streamlit.io/) (Python)
* **LLM Engine:** `Qwen/Qwen2.5-72B-Instruct` via Hugging Face Inference API.
* **Image Generation:** `stabilityai/stable-diffusion-xl-base-1.0` via Hugging Face Inference API.
* **Integration:** `huggingface_hub` Python Client.

## 💻 Installation & Setup

If you want to run this project locally:

1.  **Clone the repository**
    ```bash
    git clone [https://github.com/varelsaurus/magic-ad-generator.git](https://github.com/varelsaurus/magic-ad-generator.git)
    cd magic-ad-generator
    ```

2.  **Install dependencies**
    ```bash
    pip install -r requirements.txt
    ```

3.  **Set up API Token**
    * Create a `.streamlit/secrets.toml` file in the root directory.
    * Add your Hugging Face Token:
    ```toml
    HF_TOKEN = "your_huggingface_token_here"
    ```

4.  **Run the App**
    ```bash
    streamlit run app.py
    ```

## 👤 Author
**Varel** - *Aspiring AI Engineer*
Built with ❤️ for the Madebyhumans Internship Application.
