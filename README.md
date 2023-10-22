# Essence
[![pypiv](https://img.shields.io/pypi/v/essence-nlp.svg)](https://pypi.python.org/pypi/essence-nlp)
[![pyv](https://img.shields.io/pypi/pyversions/essence-nlp.svg)](https://pypi.python.org/pypi/essence-nlp)
[![Licence](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/jashdubal/essence/blob/main/LICENSE)
[![Downloads](https://pepy.tech/badge/essence-nlp)](https://pepy.tech/project/essence-nlp)

Essence is string processing library designed for advanced Natural Language Processing (NLP) and Generative AI tasks. Built in Rust, bridged to Python.

## Features
- **Error Correction**: Enhances text accuracy by correcting spelling and grammatical errors
- **Noise Removal**: Eliminates irrelevant information, aiding in cost-effective prompt handling especially when using APIs with usage-based pricing
- **Keyword Extraction**: Extracts key terms from prompts facilitating fast searches, database lookups, and other system interactions
- **Prompt Compression**: Reduces operational costs in AI-driven platforms by minimizing the text data processed
- **High Performance**: Leverages Rust's memory safety and speed for string processing

## Installation

Before installing Essence, ensure that you have Rust and Python installed on your system.

1. Install Rust:
   - Visit [https://rustup.rs/](https://rustup.rs/) and follow the instructions.

2. Install Python:
   - Download and install Python from [https://www.python.org/downloads/](https://www.python.org/downloads/).

3. Install Essence via pip:
```bash
pip install essence-nlp
# or
pip3 install essence-nlp
```

## Usage

```python
from essence_nlp import processing

sentence = 'Hello i am sogtware engineer, and i designing smart mashine learning system.'

# Example 1: Correcting text
corrected_sentence = processing.corrected(sentence)
print(corrected_sentence)  # Output: 'hello i am software engineer and i'm designing smart machine learning system'

# Example 2: Cleaning text
clean_sentence = processing.cleaned(sentence)
print(clean_sentence)  # Output: 'hello software engineer im designing smart machine learning system'

# Example 3: Extracting keywords
keywords = processing.keywords(sentence)
print(keywords)  # Output: 'im designing smart machine learning system: 36\nsoftware engineer: 4\nhello: 1'
```

## Benchmarks
Coming soon...

## Credits
- [nlprule](https://github.com/bminixhofer/nlprule)
- [RAKE](https://github.com/csurfer/rake-nltk)