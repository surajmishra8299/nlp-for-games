# 🧙‍♂️ Fantasy Text Generator for Games 🎮

This project uses **GPT-2** from Hugging Face to generate fantasy-themed content for games, such as:

- 🧾 Quests
- 🧱 Item descriptions
- 🧍 Character names and lore

It is lightweight, CPU-friendly, and can run on **Google Colab** without requiring a GPU.

---

## ✨ Features

- 🔮 Prompt-based fantasy text generation
- 🧪 Supports different parameters:
  - `temperature` (creativity)
  - `seed` (for reproducibility)
  - `max_length` (text size)
- ⚙️ Flask API with `/generate` endpoint (via `flask_ngrok`)
- 📂 Sample outputs and experiments included
- 💻 Runs on Colab — no setup needed

---

## 🚀 Getting Started

### 1. Open in Google Colab

> [Click here to open in Colab](https://colab.research.google.com/)  
> Upload the file `[fantasy_text_generator.ipynb](https://colab.research.google.com/drive/1PmKsNCB4jK8lpP_Iv1X31xh2bsZx_tVP?usp=sharing)`

### 2. Run the cells

- First, install dependencies:
  
```python

!pip install flask-ngrok flask transformers torch
Then run the Flask app cell.

3. Test the API
Open this in your browser:

ruby
Copy code
https://xxxx.ngrok.io/generate?prompt=Item:+A+magical+sword&temp=0.8&seed=42

🧪 Example Outputs
Prompt:
vbnet
Copy code
Item: A sword made from
Temperature	Output
0.7	A sword made from dragon bone, said to cut through armor with ease...
1.0	A sword made from the forgotten magic of the Ancients, glowing with red light...
1.3	A swirling sword forged from moonlight, blessed by a time-witch...

🔍 Parameters
Parameter	Description
prompt	The text that guides the generation
temperature	Creativity of output (higher = more random)
seed	Controls randomness for reproducibility
max_length	Max length of generated text

📦 File Structure
bash
Copy code
nlp-for-games/
├── app.py                        # Flask API (optional if using Colab only)
├── fantasy_text_generator.ipynb # Main notebook (Google Colab)
├── outputs/
│   └── outputs.txt              # Sample generated outputs
├── README.md                    # This file
├── results.md                   # Parameter experiments & observations
└── requirements.txt             # Python dependencies
🧠 Observations
See results.md for more details.

Higher temperature → more creative but unpredictable results

Same seed → same output for reproducibility

Prompt changes lead to completely different narratives

🛠️ Future Improvements
Fine-tune GPT-2 on fantasy datasets (like The Witcher, DnD, LOTR)

Add frontend UI for interactive use

Add bulk generation and download options

Host permanently on Render or Hugging Face Spaces

🧑‍💻 Dependencies
Python 3.x

Flask + Flask-Ngrok

Hugging Face Transformers

PyTorch

Install with:

bash
Copy code
pip install flask flask-ngrok torch transformers

📬 Contact
👤 Created by Suraj Mishra
📧 Email: surajmishra388495@gmail.com
