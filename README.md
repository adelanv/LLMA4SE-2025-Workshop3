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


#### Alternative 2: Run on local machine 

**Required**: Git, Docker Desktop, VSCode

1) Clone the GitHub repository on your computer from following link:

```
git clone https://github.com/adelanv/LLMA4SE-2025-Workshop3.git
```

2) Install Docker Desktop on your computer, following the link: https://www.docker.com/%20products/docker-desktop/ then run Docker Desktop.

3) Open a terminal, navigate to the repository directory where the *docker-compose.yml* file is located and run the following command:

```
docker-compose up -d
```
This is done to start all the containers, build images, and set up volumes. 

4) Open an editor and run the code blocks in a Jupyter Notebook-friendly editor (such as VSCode).
____________________________________________________________________

###  Virtual Environment

#### Alternative 1: Run on cloud - **Followed in this workshop!**
Everything is pre-set up already in Google Colab.


#### Alternative 2: Run on local machine 
Requires creating an virtual environment with Python version > 3.10.x preinstalled.








