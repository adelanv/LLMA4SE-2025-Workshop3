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

4) Create a free Neo4j AuraDB account following the link provided: https://neo4j.com/docs/aura/classic/. This is done to obtain a cloud-based, personal database instance for the experiments.

**Very important**: Once you have your credentials, you should see a popup saying “Save your password now” (they only show it once!). Copy the password and save it somewhere accessible. We will need it later. 

Lastly, open the Neo4J Aura Console and navigate to *Data services/Instances*. Create a new database instance (if not automatically created). 


### Alternative 2: Run on local machine

**Required**: Git, Docker Desktop, VSCode, *Ollama (*for local models)

1) Clone the GitHub repository on your computer from following link:

```
git clone https://github.com/adelanv/LLMA4SE-2025-Workshop3.git
```

2) Make sure Python >3.10 is installed on your machine, and is on your PATH
   ```https://realpython.com/add-python-to-path/```
   

3) Create a virtual environment to ensure the correct dependencies
    3.1) Using pip
   ```bash
    python3 -m venv .venv

    # For linux
   source .venv/bin/activate
    # On windows the activate script is located under the ./venv/Scripts/ folder, so with powershell:
   .\.venv\Scripts\activate

    # Or with git bash if installed

   source ./.venv/Scripts/activate
    ```
    3.2) Using uv

   ```bash
   uv sync
       # For linux
   source .venv/bin/activate
    # On windows the activate script is located under the ./venv/Scripts/ folder, so with powershell:
   .\.venv\Scripts\activate

    # Or with git bash if installed

   source ./.venv/Scripts/activate
    ```

4) Install Docker Desktop on your computer, following the link: https://www.docker.com/%20products/docker-desktop/ then run Docker Desktop.

5) Open a terminal, navigate to the repository directory where the *docker-compose.yml* file is located and run the following command:

```
docker-compose up -d
```
6) Run the code blocks in a Jupyter Notebook-friendly editor or with jupyter lab

    5.1) [Visual Studio Code](https://code.visualstudio.com/) (Recommended)
        Open the project folder and set the virtual environment as the default interpreter.

    5.2) If Jupyter Lab is installed

       ```bash
        jupyter lab

       ```
    or if you need to specify python version (for example version 3.11):

   ```bash
   py -3.11 -m jupyter lab

   ```
____________________________________________________________________









