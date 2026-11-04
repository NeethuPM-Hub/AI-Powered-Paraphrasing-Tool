# AI-Powered Paraphrasing Tool

## Project Overview

The **AI-Powered Paraphrasing Tool** is a Python-based application developed using Deep Learning and Natural Language Processing (NLP) techniques. It generates alternative versions of user-provided text while attempting to preserve the original meaning.

The application uses a pre-trained T5 Transformer model from Hugging Face to generate paraphrases. It also integrates grammar and spelling checking and evaluates the generated text using different quality metrics.

## Features

- AI-based text paraphrasing using a pre-trained T5 model.
- Generates multiple paraphrased versions of the input text.
- Text preprocessing and input validation.
- Grammar and spelling checking using LanguageTool.
- Automatic grammar correction.
- Semantic similarity evaluation using Sentence Transformers.
- Fluency estimation based on grammar-checking results.
- Originality estimation using TF-IDF and cosine similarity.
- Interactive Python console interface.

## Technologies Used

- Python
- Deep Learning
- Natural Language Processing (NLP)
- Hugging Face Transformers
- T5 Transformer Model
- Sentence Transformers
- LanguageTool
- Scikit-learn
- BLEU and ROUGE evaluation metrics
- Google Colab

## Pre-trained Models

**Paraphrasing Model:** `humarin/chatgpt_paraphraser_on_T5_base`

**Semantic Similarity Model:** `sentence-transformers/all-MiniLM-L6-v2`

## Project Workflow

1. Accept text input from the user.
2. Validate and preprocess the input.
3. Generate multiple paraphrased versions using the T5 model.
4. Allow the user to select a preferred paraphrase.
5. Check grammar and spelling using LanguageTool.
6. Apply available grammar corrections.
7. Evaluate the selected paraphrase using semantic similarity, fluency and lexical originality indicators.

## Evaluation Metrics

| Metric | Purpose |
|---|---|
| Semantic Similarity | Estimates how closely the paraphrased text relates in meaning to the original. |
| Fluency Score | Provides a simple estimate based on detected grammar issues. |
| Originality Score | Estimates lexical difference using TF-IDF and cosine similarity. |
| BLEU | Measures n-gram overlap with reference paraphrases. |
| ROUGE | Measures word and sequence overlap with reference paraphrases. |

*Note: BLEU and ROUGE require suitable reference paraphrases. Semantic similarity, fluency and originality scores are indicators and should not be interpreted as definitive measures of meaning preservation, writing quality or plagiarism.*

## Installation

Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/AI-Powered-Paraphrasing-Tool.git
```

Install the dependencies:

```bash
pip install -r requirements.txt
```

Open the notebook using Google Colab or Jupyter Notebook.

## Sample Input

```text
RPA is a form of business process automation technology to build software robots to automate tasks and mimic the human interaction with software.
```

## Sample Output

The application generates multiple paraphrased alternatives and allows the user to select a preferred version for grammar checking and quality evaluation.

## Future Enhancements

- Improve diversity among generated paraphrases.
- Add duplicate-output detection.
- Improve meaning preservation and evaluation.
- Develop a web-based user interface.
- Support multiple languages.

## Author

Developed as part of a Deep Learning project to explore Transformer-based Natural Language Processing applications.
