# Workshop: Multi-Agent LLMs and Knowledge Graphs for Monitoring and Sustaining Software Systems


## Environment Setup 

____________________________________________________________________
### How to run?
We present two options to run the experiments below, using cloud resources and hosted database instance or running locally using Docker containers (for local models, Ollama configuration is provided). For simplicity, this workshop walkthorough will be run on the cloud.

#### Alternative 1: Run on cloud - **Followed in this workshop!**

**Required**: Google account, Neo4J Aura account

1) Go to Google Colab (https://colab.google/) and click on Open Colab.

2) Sign in with your Google account.

3) Open the invitation link (TODO: ADD). In the menu bar, go to File → Save a copy in Drive. This will create your own personal copy of the notebook.

4) Go to step **Connect to Neo4J and Verify Setup** below to connect to your graph database. 


### Alternative 2: Run on local machine

1) Make sure python >3.10 is installed on your machine, and is on your PATH
   ```https://realpython.com/add-python-to-path/```
   
1) Save the workshop directory content locally on your machine or clone the GitHub repository:

```
git clone https://github.com/adelanv/LLMA4SE-2025-Workshop3.git
```

2) Create a virtual environment to ensure the correct dependencies
    2.1) Using pip
   ```bash
    python3 -m venv .venv

    # For linux
   source .venv/bin/activate
    # On windows the activate script is located under the ./venv/Scripts/ folder, so with powershell:
   .\.venv\Scripts\activate

    # Or with git bash if installed

   source ./.venv/Scripts/activate
    ```
    2.2) Using uv

   ```bash
   uv sync
       # For linux
   source .venv/bin/activate
    # On windows the activate script is located under the ./venv/Scripts/ folder, so with powershell:
   .\.venv\Scripts\activate

    # Or with git bash if installed

   source ./.venv/Scripts/activate
    ```

   
2) Inside the directory create a *openaiapi.ini* file, add the following lines, and replace with your OpenAI API key:

```
[openai]
OPENAI_API_KEY = sk-xxxx-xxxx ...
```
Inside the notebook, you may add the following code to access your OpenAI API key:

```
import configparser

config = configparser.ConfigParser(allow_no_value = True)
config.read('openaiapi.ini')
openai_api_key = config.get('openai', 'OPENAI_API_KEY')
```

3) Install Docker Desktop on your computer, following the link: https://www.docker.com/%20products/docker-desktop/ then run Docker Desktop.

6) Open a terminal, navigate to the repository directory containing the *docker-compose.yml* file and run the following command:

```
docker-compose up -d
```
5) Run the code blocks in a Jupyter Notebook-friendly editor or with jupyter lab
    5.1) Visual Studio Code
        Open the project folder and set the virtual environment as the default interpreter.

    5.2) If jupyter lab is installed

       ```bash
        jupyter lab

       ```
    or if you need to specify python version (for example version 3.11):

   ```bash
   py -3.11 -m jupyter lab

   ```

7) 
____________________________________________________________________

###  Virtual Environment

#### Alternative 1: Run on cloud - **Followed in this workshop!**
Everything is pre-set up already in Google Colab.


#### Alternative 2: Run on local machine 
Requires creating an virtual environment with Python version > 3.10.x preinstalled.








