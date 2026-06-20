# GPT-Style LLM from Scratch

> "What I cannot create, I do not understand." — Richard Feynman

Welcome to my implementation of a GPT-style Large Language Model built from scratch using PyTorch. This project follows the architecture and training methodology presented in Sebastian Raschka's *Build a Large Language Model (From Scratch)*. The project demonstrates the complete workflow of building, training, saving, loading, and interacting with a transformer-based language model from the ground up.

---

## Getting Started

Follow the steps below to set up your local development environment and run the model.

### 1. Clone the Repository

```bash
git clone <your-repository-url>
cd GPT-Style-LLM-From-Scratch
```

### 2. Prerequisites

Ensure Python is installed on your system.

```bash
python --version
```

Recommended version:

```text
Python 3.10+
```

### 3. Set Up a Virtual Environment

This project uses `uv` for fast and efficient package management.

#### Install uv

```bash
pip install uv
```

#### Create a Virtual Environment

```bash
uv venv --python=python3.10
```

#### Activate the Environment

##### Windows

```bash
.venv\Scripts\activate
```

##### Linux / macOS

```bash
source .venv/bin/activate
```

### 4. Install Dependencies

```bash
uv pip install packaging
uv pip install -r requirements.txt
```

If you encounter dependency-related issues, reinstall the problematic package separately:

```bash
uv pip install <package_name>
```

### 5. Verify the Environment

Run the following command to verify that your environment has been configured correctly:

```bash
python python_environment_check.py
```

---

## Running the Project

### Save and Load Model Weights

Generate and save model weights:

```bash
python save_model.py
```

### Launch the Chat Interface

Start the Chainlit application:

```bash
chainlit run app.py
```

After launching, open the local URL displayed in the terminal and interact with the model through the web interface.

---

## Features

* GPT-style transformer architecture implemented from scratch
* Tokenization and text generation pipeline
* Multi-Head Self-Attention mechanism
* Feed Forward Neural Networks
* Layer Normalization
* Residual Connections
* Model weight saving and loading
* Interactive chatbot interface using Chainlit
* PyTorch-based implementation
* Modular and extensible codebase

---

## Project Structure

```text
GPT-Style-LLM-From-Scratch/
│
├── app.py
├── save_model.py
├── python_environment_check.py
├── requirements.txt
├── notebooks/
├── data/
├── models/
└── README.md
```

---

## Tech Stack

### Framework

* PyTorch

### User Interface

* Chainlit

### Package Management

* uv

### Programming Language

* Python

---

## Learning Objectives

This project was built to gain a deeper understanding of:

* Transformer architectures
* Attention mechanisms
* Token embeddings and positional encodings
* Language model training pipelines
* Text generation techniques
* PyTorch internals
* Building production-style AI applications

---

## Project Author

**Harsh**

---

## Acknowledgements

This project is inspired by the work of Sebastian Raschka and serves as a practical implementation of the concepts presented in his book:

**Build a Large Language Model (From Scratch)**

Special thanks to Sebastian Raschka for providing an excellent educational resource for understanding modern language models from first principles.
