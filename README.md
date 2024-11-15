# Genre-Specific Story Generator

This project fine-tunes GPT-Neo on genre-specific datasets to create customized stories based on user input. It uses a Gradio interface to provide an interactive platform for generating stories.

---

## 📋 Features

- Fine-tunes GPT-Neo for genre-specific text generation.
- Interactive user interface using **Gradio**.
- Generates stories based on user-selected genre, prompt, and word count.
- Implements advanced text generation techniques (e.g., **nucleus sampling**, **temperature control**, and **no-repeat n-grams**).
- Evaluates text readability using **Flesch Reading Ease** and **Flesch-Kincaid Grade**.

---

## 🛠️ Tech Stack

- **Python**: Core programming language.
- **PyTorch**: For handling the GPT-Neo model.
- **Transformers Library**: From Hugging Face, used for GPT-Neo and tokenizer.
- **Gradio**: Interactive web-based UI.
- **NLTK**: For natural language processing (tokenization, POS tagging, etc.).
- **Textstat**: For text readability metrics.
- **Google Drive Integration**: Used to store fine-tuned models and outputs.

---

## 🚀 Installation and Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/astralranger/story-generator.git
   cd story-generator

---

Set up the fine-tuned models:

Save your fine-tuned models in a directory (e.g ./drive/MyDrive/fine_tuned_models/) following the folder structure: <genre_name>/.

Run the Gradio app:

```bash
  python app.py
```
Access the app on your browser at http://127.0.0.1:7860.

---

## 🧑‍💻 Usage

1. Select a **genre** from the dropdown menu.
2. Enter a **prompt** (e.g., "A hero ventures into a mysterious forest").
3. Set a desired **word count**.
4. Click **Generate Story** to create a customized story.
5. The story will be displayed in the app and saved to `/MyDrive/outputs/<genre>_story_output.txt`.

---

## 📊 Key Concepts

### GPT-Neo Fine-Tuning

Fine-tuned on genre-specific datasets to adapt the model for better genre alignment.

### Training Arguments

The fine-tuning process leverages specific configurations:

- **Batch Size**: Controls memory usage during training.
- **Gradient Accumulation**: Accumulates gradients over multiple steps to handle large datasets.
- **Epochs**: Multiple passes over the data to refine the model.

