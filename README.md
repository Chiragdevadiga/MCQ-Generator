# MCQ Generation Using NLP

This project aims to automate the generation of multiple-choice questions (MCQs) using natural language processing (NLP). The system generates MCQs from textual sources, creating questions, correct answers, and plausible distractors. It utilizes various NLP techniques and libraries to streamline the process of creating educational assessments, quizzes, and training materials.

## Features
- **Text Summarization**: Summarize input text to extract key information.
- **Keyword Extraction**: Identify significant keywords and phrases for question generation.
- **Question Generation**: Use the T5 model to generate questions based on context and keywords.
- **Distractor Creation**: Generate plausible distractors using Sense2Vec, WordNet, and ConceptNet.
- **User-Friendly Interface**: Gradio-based interface for easy interaction and MCQ generation.

## Installation
To run this project, you need Python 3.6 or higher. You can install the required dependencies using the following commands:

```bash
# Install core dependencies
pip install flashtext==2.7
pip install git+https://github.com/boudinfl/pke.git
pip install transformers==4.28.1
pip install sentencepiece==0.1.95
pip install textwrap3==0.9.2
pip install gradio==3.9
pip install strsim==0.0.3
pip install sense2vec==2.0.1
pip install sentence-transformers==2.2.2
```
Additionally, ensure that NLTK data is downloaded for the project to run smoothly:

```bash
# Download NLTK data
import nltk
nltk.download('punkt')
nltk.download('stopwords')
nltk.download('wordnet')
```
## Usage
To use the automated MCQ generation system, follow these steps:

- Input Text: Provide a paragraph or larger text from which you want to generate MCQs.
- Summarize Text: Use the T5 model to summarize the input text.
- Extract Keywords: Identify significant keywords from the summarized text.
- Generate Questions: Create questions using the extracted keywords and summarized text.
- Generate Distractors: Use Sense2Vec, WordNet, or ConceptNet to create plausible distractors.
- Gradio Interface: Launch the Gradio-based user interface to interact with the system.
