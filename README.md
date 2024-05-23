# Running Ollama in GitHub Codespaces
Learn how to efficiently run Ollama in GitHub Codespaces for free.

## What is a Codespace?
A codespace is a cloud-hosted development environment tailored for coding. GitHub Codespaces allows you to customize your project by committing configuration files to your repository, creating a consistent and repeatable environment for all users. For more details, refer to the [Introduction to dev containers](https://docs.github.com/en/codespaces/setting-up-your-project-for-codespaces/adding-a-dev-container-configuration/introduction-to-dev-containers).

## What is Ollama?
Ollama is an open-source project designed to simplify running Large Language Models (LLMs) on local machines. It provides a user-friendly interface and functionality to make advanced AI accessible and customizable.

## Setting Up Ollama in GitHub Codespaces

Follow these steps to set up and run Ollama in a GitHub Codespace:

### 1. Open a Codespace
- Navigate to your repository on GitHub.
- Click on the `Code` button and select `Open with Codespaces`.
- If you don't have an existing codespace, create a new one.

### 2. Install Ollama
- Open the terminal in your codespace.
- Run the following command to download and install Ollama:
  ```sh
  curl -fsSL https://ollama.com/install.sh | sh
  ```

### 3. Verify the Installation
- Type `ollama` in the terminal to verify the installation:
  ```sh
  ollama
  ```
- If the installation is successful, you will see a list of available Ollama commands.

### 4. Start Ollama
- Run the following command to start Ollama:
  ```sh
  ollama serve
  ```

### 5. Run and Chat with Llama 3
- To run and interact with the Llama 3 model, use the following command:
  ```sh
  ollama run llama3
  ```

## Ollama Model Library

Ollama provides a variety of models that you can download and use. Visit the [Ollama model library](https://ollama.com/library) for a complete list.

### Example Models

Here are some example models available for use:

| Model              | Parameters | Size  | Command                       |
| ------------------ | ---------- | ----- | ----------------------------- |
| Llama 3            | 8B         | 4.7GB | `ollama run llama3`           |
| Llama 3            | 70B        | 40GB  | `ollama run llama3:70b`       |
| Phi 3 Mini         | 3.8B       | 2.3GB | `ollama run phi3`             |
| Phi 3 Medium       | 14B        | 7.9GB | `ollama run phi3:medium`      |
| Gemma              | 2B         | 1.4GB | `ollama run gemma:2b`         |
| Gemma              | 7B         | 4.8GB | `ollama run gemma:7b`         |
| Mistral            | 7B         | 4.1GB | `ollama run mistral`          |
| Moondream 2        | 1.4B       | 829MB | `ollama run moondream`        |
| Neural Chat        | 7B         | 4.1GB | `ollama run neural-chat`      |
| Starling           | 7B         | 4.1GB | `ollama run starling-lm`      |
| Code Llama         | 7B         | 3.8GB | `ollama run codellama`        |
| Llama 2 Uncensored | 7B         | 3.8GB | `ollama run llama2-uncensored`|
| LLaVA              | 7B         | 4.5GB | `ollama run llava`            |
| Solar              | 10.7B      | 6.1GB | `ollama run solar`            |

>**Important:**
> Ensure that your system meets the following RAM requirements:
> - At least 8 GB of RAM for 7B models
> - At least 16 GB of RAM for 13B models
> - At least 32 GB of RAM for 33B models

By following these steps, you can set up and run Ollama efficiently within GitHub Codespaces, leveraging its cloud-based environment to explore and utilize powerful LLMs.
