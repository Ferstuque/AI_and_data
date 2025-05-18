# AI_and_data

This repository contains applications and Google Colab notebooks and resources focused on Artificial Intelligence (AI) and data science projects.

## Application

### [Ai-Powered Data Parsing](https://huggingface.co/spaces/Feralves/data_parsing)

## EN

# Data Insights with AI: Unlock the Power of Your CSV Files

Dive into your data with ease! This Hugging Face Space provides a user-friendly application to analyze your `.CSV` files using the power of artificial intelligence. Simply upload your data, ask your questions in natural language, and watch as the AI uncovers valuable insights and even provides the Python code used for the analysis.

## How to Use

1.  **Upload Your CSV File:** Click the "Upload a CSV file" button and select the `.CSV` file you want to analyze.
2.  **Ask Your Questions:** In the text box, type any questions you have about your data. For example:
    * "What are the top 5 products by sales?"
    * "What is the average age in this dataset?"
    * "Show me a distribution of the 'price' column."
    * "Are there any correlations between 'feature A' and 'feature B'?"
3.  **Get AI-Powered Insights:** The AI will process your data and provide you with:
    * **Concise answers** to your questions.
    * **Key insights** and observations about your data.
    * **Python code** that was used to perform the analysis, allowing you to reproduce and further explore the results.

## Example Files

Get started quickly by trying out these example `.CSV` files:

* `vendas.csv`: A sample dataset of sales transactions.
* `spam.csv`: A dataset for spam detection analysis.
* `campeonato_brasileir.csv`: Data from the Brazilian football league.
* `bicicleta.csv`: Information related to bicycle usage or sales.

You can upload these files directly into the application to see it in action!

## Behind the Scenes

This application leverages the power of AI and Python data analysis libraries (like Pandas, etc.) through a Gradio interface. The AI model is designed to understand your questions and generate relevant analysis and code snippets.

## Configuration Reference

For more advanced configuration options and details about Hugging Face Spaces, please refer to the official documentation: [https://huggingface.co/docs/hub/spaces-config-reference](https://huggingface.co/docs/hub/spaces-config-reference)

---

## PT-BR

# Insights de Dados com IA: Desbloqueie o Poder dos Seus Arquivos CSV

Mergulhe nos seus dados com facilidade! Este Space do Hugging Face oferece um aplicativo amigável para analisar seus arquivos `.CSV` usando o poder da inteligência artificial. Basta enviar seus dados, fazer suas perguntas em linguagem natural e observar enquanto a IA descobre insights valiosos e até fornece o código Python usado para a análise.

## Como Usar

1.  **Envie Seu Arquivo CSV:** Clique no botão "Upload a CSV file" e selecione o arquivo `.CSV` que você deseja analisar.
2.  **Faça Suas Perguntas:** Na caixa de texto, digite qualquer pergunta que você tenha sobre seus dados. Por exemplo:
    * "Quais são os 5 principais produtos por vendas?"
    * "Qual é a idade média neste conjunto de dados?"
    * "Mostre-me uma distribuição da coluna 'price'."
    * "Existem correlações entre 'feature A' e 'feature B'?"
3.  **Obtenha Insights com IA:** A IA processará seus dados e fornecerá:
    * **Respostas concisas** às suas perguntas.
    * **Insights e observações** importantes sobre seus dados.
    * **Código Python** que foi usado para realizar a análise, permitindo que você reproduza e explore ainda mais os resultados.

## Arquivos de Exemplo

Comece rapidamente experimentando estes arquivos `.CSV` de exemplo:

* `vendas.csv`: Um conjunto de dados de amostra de transações de vendas.
* `spam.csv`: Um conjunto de dados para análise de detecção de spam.
* `campeonato_brasileir.csv`: Dados do campeonato brasileiro de futebol.
* `bicicleta.csv`: Informações relacionadas ao uso ou vendas de bicicletas.

Você pode enviar esses arquivos diretamente no aplicativo para vê-lo em ação!

## Por Trás dos Panos

Este aplicativo aproveita o poder da IA e das bibliotecas de análise de dados do Python (como Pandas, etc.) através de uma interface Gradio. O modelo de IA é projetado para entender suas perguntas e gerar análises e trechos de código relevantes.

## Referência de Configuração

Para opções de configuração mais avançadas e detalhes sobre os Spaces do Hugging Face, consulte a documentação oficial: [https://huggingface.co/docs/hub/spaces-config-reference](https://huggingface.co/docs/hub/spaces-config-reference)


________________________________

## Notebook

### `LLM - GPT2 - Fine-Tuning - HuggingFace dataset.ipynb`

This notebook demonstrates the process of fine-tuning a small pre-trained Language Model (LLM), specifically GPT-2, using a dataset from the Hugging Face Datasets library. **Designed for execution on Google Colab with GPU acceleration for enhanced performance.**

**Key aspects covered in the notebook:**

* **Google Colab Optimization:** Instructions and code snippets optimized for running seamlessly on Google Colab, including GPU utilization.
* **Dataset Loading:** Guidance on how to efficiently load a text-based dataset from the Hugging Face Hub within the Colab environment.
* **Model Loading:** Loading the pre-trained GPT-2 Small model from the Hugging Face Transformers library.
* **Tokenization:** Preprocessing the text data using the appropriate tokenizer for GPT-2.
* **Fine-Tuning:** Implementing the fine-tuning process using the Transformers Trainer API, leveraging the GPU cluster available in Colab for faster training times.
* **Evaluation:** Analysis of the model's performance **before** fine-tuning on a specific task (e.g., text generation, next word prediction).
* **Post Fine-Tuning Analysis:** Evaluation of the model's performance **after** fine-tuning, highlighting the improvements or changes in its capabilities.
* **Comments and Explanations:** Detailed comments throughout the code explaining each step, the reasoning behind it, and considerations for running on Colab.

## Getting Started

To run the notebooks in this repository, particularly the LLM fine-tuning notebook, it is **highly recommended** to use Google Colab to take advantage of its free GPU resources.

1.  **Open in Google Colab:** Navigate to the `LLM - GPT2 - Fine-Tuning - HuggingFace dataset.ipynb` file in this repository and click the "Open in Colab" button (if available on the platform you are viewing this README). Alternatively, you can upload the `.ipynb` file to your Google Drive and open it with Google Colaboratory.

2.  **Connect to a GPU:** Once the notebook is open in Colab, go to "Runtime" in the menu bar and select "Change runtime type." In the "Hardware accelerator" dropdown, choose "GPU." This will allocate a GPU to your Colab session, significantly speeding up the fine-tuning process.

3.  **Install Libraries (if necessary):** The notebook itself will likely contain code to install the required libraries. However, if you encounter any missing library errors, you can install them directly in the Colab notebook using `pip`:

    ```python
    !pip install transformers datasets accelerate evaluate bert-score nltk
    !pip install git-lfs
    ```

4.  **Follow the Notebook:** Execute the cells in the notebook sequentially, reading the comments and explanations to understand each step of the fine-tuning process.

## Usage

The primary notebook in this repository is designed to be self-contained and provides a step-by-step guide to fine-tuning GPT-2 on a Hugging Face dataset within the Google Colab environment. Simply open the notebook in Colab and execute the cells.

## Contributions

Contributions to this repository are welcome. If you find any issues, have suggestions for improvements (especially regarding Colab optimization or alternative approaches), please feel free to open a pull request or submit an issue.

