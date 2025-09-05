# **mini-rag-app**

A minimal implementation of a RAG model for Question Answering.

## Requirements

- Python 3.8 or later

## Install Python using Miniconda

1. **Download and install Miniconda:**  
    [Miniconda Download (Linux x86_64)](https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh)

2. **Create a new environment:**
    ```bash
    conda create -n mini-rag python=3.10
    ```

3. **Activate the environment:**
    ```bash
    conda activate mini-rag
    ```
### (Optional) Setup your command line for better readability

```bash
export PS1="\[\033[01;32m\]\u@\h:\w\n\[\033[00m\]\$ "
```
## Installation

1. **Install the required packages:**
    ```bash
    pip install -r requirements.txt
    ```

2. **Set up environment variables:**
    ```bash
    cp .env.example .env
    ```
    Edit the `.env` file to set your environment variables, such as `OPENAI_API_KEY`.

3. **Run Alembic migrations:**
    ```bash
    alembic upgrade head
    ```

## Run the FastAPI server
     ```bash
    $ uvicorn main:app --reload --host 0.0.0.0 --port 5000
    ```