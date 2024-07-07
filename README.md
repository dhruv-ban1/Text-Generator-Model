# Markov Chain Text Generator

## Table of Contents

1. [Introduction](#introduction)
2. [Features](#features)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Configuration](#configuration)
6. [Examples](#examples)
7. [Contribution](#contribution)
8. [License](#license)
9. [Contact](#contact)

---

## Introduction

The Markov Chain Text Generator is a Python-based tool that generates text based on a Markov Chain model. Markov Chains are mathematical systems that transition from one state to another, with the probability of each transition depending solely on the current state. This model is particularly useful for generating coherent and somewhat meaningful sequences of text that resemble the input corpus.

## Features

- **Text Generation**: Create new sentences or paragraphs based on an input corpus.
- **Customizable Order**: Set the order of the Markov Chain to control the complexity and coherence of the generated text.
- **Flexible Input**: Easily feed in different text corpora to generate varied outputs.
- **Output Diversity**: Generate multiple unique outputs based on the same input corpus.

## Installation

### Prerequisites

- Python 3.7 or higher
- pip (Python package installer)

### Steps

1. Clone the repository:

    ```bash
    git clone https://github.com/username/markov-chain-text-generator.git
    cd markov-chain-text-generator
    ```

2. Create and activate a virtual environment (optional but recommended):

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install the required dependencies:

    ```bash
    pip install -r requirements.txt
    ```

## Usage

To generate text using the Markov Chain model, follow these steps:

1. Prepare your text corpus. This is the input text from which the model will learn the structure and generate new text.

2. Run the script with the desired parameters:

    ```bash
    python markov_chain_text_generator.py --input path/to/corpus.txt --order 2 --length 100
    ```

    **Parameters:**
    - `--input`: Path to the input text file.
    - `--order`: The order of the Markov Chain (number of previous words considered).
    - `--length`: Number of words in the generated text.

3. The generated text will be displayed in the console. You can also direct the output to a file using redirection:

    ```bash
    python markov_chain_text_generator.py --input path/to/corpus.txt --order 2 --length 100 > generated_text.txt
    ```

## Configuration

You can adjust the settings of the Markov Chain model through the command line parameters or by editing the `config.json` file:

```json
{
    "input": "path/to/corpus.txt",
    "order": 2,
    "length": 100
}
