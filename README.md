# txtai: AI-powered search engine

[![Version](https://img.shields.io/github/release/neuml/txtai.svg?style=flat&color=blue)](https://github.com/neuml/txtai/releases)
[![GitHub Release Date](https://img.shields.io/github/release-date/neuml/txtai?style=flat&color=success)](https://github.com/neuml/txtai/releases)
[![GitHub issues](https://img.shields.io/github/issues/neuml/txtai?style=flat&color=blue)](https://github.com/neuml/txtai/issues)
[![GitHub last commit](https://img.shields.io/github/last-commit/neuml/txtai?style=flat&color=success)](https://github.com/neuml/txtai)

txtai builds an AI-powered index over sections of text. txtai supports building text indices to perform similarity searches and create extractive question-answering based systems. 

![demo](https://raw.githubusercontent.com/neuml/txtai/master/demo.gif)

NeuML uses txtai and/or the concepts behind it to power all of our Natural Language Processing (NLP) applications. Example applications:

- [cord19q](https://github.com/neuml/cord19q) - COVID-19 literature analysis
- [paperai](https://github.com/neuml/paperai) - AI-powered literature discovery and review engine for medical/scientific papers
- [neuspo](https://neuspo.com) - a fact-driven, real-time sports event and news site
- [codequestion](https://github.com/neuml/codequestion) - Ask coding questions directly from the terminal

txtai is built on the following stack:

- [sentence-transformers](https://github.com/UKPLab/sentence-transformers)
- [transformers](https://github.com/huggingface/transformers)
- [faiss](https://github.com/facebookresearch/faiss)
- Python 3.6+

## Installation
The easiest way to install is via pip and PyPI

    pip install txtai

You can also install txtai directly from GitHub. Using a Python Virtual Environment is recommended.

    pip install git+https://github.com/neuml/txtai

Python 3.6+ is supported

### Troubleshooting
This project has dependencies that require compiling native code. Windows and macOS systems require the following additional steps. Most Linux environments will install without any additional steps.

#### Windows

- Install C++ Build Tools - https://visualstudio.microsoft.com/visual-cpp-build-tools/
- PyTorch Windows binaries are not on PyPI, the following url link must be added when installing

    ```
    pip install txtai -f https://download.pytorch.org/whl/torch_stable.html
    ```

    See [pytorch.org](https://pytorch.org) for more information.

#### macOS

- Run the following before installing

    ```
    brew install libomp
    ```

    See [this link](https://github.com/kyamagu/faiss-wheels#prerequisite) for more information.

## Examples

The examples directory has a series of examples and notebooks giving an overview of txtai. See the list of notebooks below.

### Notebooks

| Notebook     |      Description      |   |
|:----------|:-------------|------:|
| [Introducing txtai](https://github.com/neuml/txtai/blob/master/examples/01_Introducing_txtai.ipynb)  | Overview of the functionality provided by txtai  |[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/01_Introducing_txtai.ipynb) |
| [Extractive QA with txtai](https://github.com/neuml/txtai/blob/master/examples/02_Extractive_QA_with_txtai.ipynb)  | Extractive question-answering with txtai  |[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/02_Extractive_QA_with_txtai.ipynb) |
| [Build an Embeddings index from a data source](https://github.com/neuml/txtai/blob/master/examples/03_Build_an_Embeddings_index_from_a_data_source.ipynb)  | Embeddings index from a data source backed by word embeddings |[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/03_Build_an_Embeddings_index_from_a_data_source.ipynb) |
| [Extractive QA with Elasticsearch](https://github.com/neuml/txtai/blob/master/examples/04_Extractive_QA_with_Elasticsearch.ipynb)  | Extractive question-answering with Elasticsearch  |[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/04_Extractive_QA_with_Elasticsearch.ipynb) |
