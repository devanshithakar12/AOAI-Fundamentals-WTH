# Challenge 00 - Prerequisites - Ready, Set, GO!

**[Home](../README.md)** - [Next Challenge >](./Challenge-01.md)

## Introduction

Thank you for participating in the AI Fluency Event. Before you can hack, you will need to set up some prerequisites.

## Description
In this challenge, you will set up the necessary prerequisites and environment through Codespaces to complete the rest of the hack, including:

- [Setup Codespace](#setup-codespace)
- [Access Azure OpenAI](#access-azure-openai)
- [Jupyter Notebook Environment](#setup-jupyter-notebook-environment)
- [Student Resources](#student-resources)
- [Setup Azure OpenAI](#setup-azure-openai)
- [Additional Prerequisites](#additional-common-prerequisites)


### Access Azure OpenAI 

You will need an Azure subscription to complete this hack. If you don't have one, get a free trial here.
- [Azure Subscription](https://azure.microsoft.com/en-us/free/)

Before you can start the hack, you will also need to apply for access to Azure OpenAI as it is currently in high-demand.

An Azure subscription is necessary to [apply for Azure OpenAI access](https://aka.ms/oaiapply). We recommend applying as early as possible as processing times will vary, sometimes taking more than several business days.

### Setup Codespace

You will need to setup your codespace in order to view all the challenge descriptions, Jupyter Notebook files, and other needed files for this event. Here are the steps you will need to follow:

1. Your coach will provide you with the Github Repo for this hack. Please open this link and sign in with your personal Github account. Note: Make sure you do not sign in with your enterprise managed Github account.

2. Once you are signed in, click on the green "Code" button. Then click on "Codespaces". You should be able to click on the three dots. Then press "+ New with options". You can keep the default config and just ensure that the Machine Type is 2-core. Finally, hit "Create codespace". 

3. You should be able to view your codespace. Enter in the following command in the terminal: `pip install -r requirements.txt`. This should successfully install all the libraries you need.

4. Fill out your .env file with the Azure resource credentials. You can fill the values in this file as you go through the challenges.

5. You are ready to run the Jupyter Notebook files, hooray!

### Jupyter Notebook Environment 

You will be working with Jupyter Notebooks and Python to interact with Azure OpenAI.

[Jupyter Notebook](https://jupyter.org/) is an open-source web application that allows you to create and share documents containing live code, equations, visualizations, and narrative text. It's useful for a wide range of tasks, such as data cleaning and transformation, numerical simulation, statistical modeling, data visualization, and machine learning.

Jupyter notebooks require an environment to run in. You will be running these in your Codespace. Navigate to the notebooks folder and click on the Jupyter Notebook you would like to start working with for each future challenge. 

--------SKIP THIS PORTION IF USING CODESPACES-----------

#### Student Resources *SKIP IF YOU ARE USING CODESPACE, THIS IS ONLY IF YOU WANT TO SETUP YOUR ENV LOCALLY OR IN THE CLOUD*

Your coach will provide you with a `Resources.zip` file that contains resource files you will use to complete the challenges for this hack.  

These resources include Jupyter notebooks, starter code, and sample data sources. 

You should download and unpack the `Resources.zip` file there to your local workstation.  The rest of the challenges will refer to the relative paths inside the `Resources.zip` file where you can find the various resources to complete the challenges.

For the event December 7 - 8, 2023, you can download the file here: [`Resources.zip`](https://aka.ms/wthopenaifundamentalsresources)

#### Local Workstation Environment *SKIP IF YOU ARE USING CODESPACE, THIS IS ONLY IF YOU WANT TO SETUP YOUR ENV LOCALLY*

If you plan to work on your local workstation, please ensure you have the following tools and resources before hacking:
- [Python Installation](https://www.python.org/downloads), version at least \>= 3.6, the minimum requirement for using OpenAI's GPT-3.5-based models, such as ChatGPT.
- Conda Installation, for project environment management and package management, version \>= conda 4.1.6. Anaconda distribution is a popular Python distribution, while Miniconda is the lightweight version of Anaconda.
  - [Anaconda](https://docs.anaconda.com/anaconda/install) OR [Miniconda](https://docs.conda.io/en/latest/miniconda.html)
- Environment setup:
  - Open Anaconda Prompt or your favourite terminal and verify Python and Conda installations using `python --version` and `conda --version`
  - Create a project environment using Conda - `conda create --name <env_name>`
  - Activate Conda environment - `conda activate <env_name>`
  - Install required libraries and packages, provided in the form of a `requirements.txt` file in the `Resources/Notebooks` section of the zip folder. We recommend using pip or Conda in a virtual environment to do so. For example, you can run `pip install -r requirements.txt`
  - Open the project in VS Code using `code .`
  - If you are using Visual Studio Code, make sure you change your Python interpreter (CTRL+SHIFT+P) to select the project/virtual environment that you just created.

For more information, see [Jupyter Notebooks in VS Code](https://code.visualstudio.com/docs/datascience/jupyter-notebooks)

#### Cloud Environment *SKIP IF YOU ARE USING CODESPACE, THIS IS ONLY IF YOU WANT TO SETUP YOUR ENV IN THE CLOUD*

If you are not interested or able to set up a Jupyter Notebook environment on your local workstation, you can set one up in the cloud with Azure Machine Learning Studio and take advantage of Azure Compute power. 

For more information, see: [Run Jupyter Notebooks in your Workspace](https://learn.microsoft.com/en-us/azure/machine-learning/how-to-run-jupyter-notebooks?view=azureml-api-2)

Once you have an Azure Machine Learning Studio Workspace set up, you can upload the contents of the `/Notebooks` folder in your `Resources.zip` file to it. For more information on this, see: [How to create and manage files in your workspace](https://learn.microsoft.com/en-us/azure/machine-learning/how-to-manage-files?view=azureml-api-2)

--------END SKIP SECTION---------------

### Setup Azure OpenAI

Once you have set up a Jupyter notebook environment, you create an Azure OpenAI resource and do some initial configuration.

- [Create an Azure OpenAI Resource](https://learn.microsoft.com/en-us/azure/ai-services/openai/how-to/create-resource?pivots=web-portal) 
- Deploy the following models in your Azure OpenAI resource.
  - `gpt-35-turbo`
  - `text-embedding-ada-002`
    - **NOTE:** A couple of challenges may require a few additional prerequisites so be sure to check those out in the respective challenges. 
- Add required credentials of Azure resources in the  `.env` file, which should be visible in your codespace. You can get these credentials through the Azure Portal within your AOAI resource. Click on Keys and Endpoint from the dropdown menu on the left side. Learn more about using `.env` files [here](https://dev.to/edgar_montano/how-to-setup-env-in-python-4a83#:~:text=How%20to%20setup%20a%20.env%20file%201%201.To,file%20using%20the%20following%20format%3A%20...%20More%20items).
  - **NOTE:** Additional Azure resources such as Azure Form Recognizer (AKA Azure Document Intelligence) and Azure Cognitive Search (AKA AI Search) will be required for later challenges. 

## Additional Common Prerequisites

We have compiled a list of common tools and software that will come in handy to complete most What The Hack Azure-based hacks!

You might not need all of them for this hack you are participating in. However, if you work with Azure on a regular basis, we suggest considering having the following in your developer toolkit.

- [Visual Studio Code](../../000-HowToHack/WTH-Common-Prerequisites.md#visual-studio-code)
- [Managing Cloud Resources](../../000-HowToHack/WTH-Common-Prerequisites.md#managing-cloud-resources)
  - [Azure Portal](../../000-HowToHack/WTH-Common-Prerequisites.md#azure-portal)
  - [Azure CLI](../../000-HowToHack/WTH-Common-Prerequisites.md#azure-cli)

## Success Criteria

To complete this challenge successfully, you should be able to:

- Verify that you are able to see the following in your Codespace:
  - The challenges folder with all five challenge markdown files. These .md files will contain descriptions of the challenges. Remember to open these by right clicking on the .md file and selecting "Open Preview". Alternatively, you can also do CTRL + SHIFT + V on your Windows machine.
  - The data folder with structured and unstructured folders along with the Automobile.csv and CH3-data.pdf files. This is the data the challenges will be working with.
  - The notebooks folder with eight files. These are the Jupyter Notebook files you will run in the next few challenges.
  - The .env file where you will store all your credentials.
  - The requirements.txt file which has all the libraries you will need in order to run the Jupyter Notebooks.
- Verify that you have Python and Conda installed
- Verify that you have created the AOAI resource and deployed the necessary deployments

## Learning Resources

- [Codespaces Overview](https://docs.github.com/en/codespaces/overview)
- [Jupyter Notebooks in VS Code](https://code.visualstudio.com/docs/datascience/jupyter-notebooks)
- [Jupyter Notebooks](https://jupyter.org/)
- [Project Jupyter](https://en.wikipedia.org/wiki/Project_Jupyter)
- [Run Jupyter Notebooks In Your (Azure Machine Learning) Workspace](https://learn.microsoft.com/en-us/azure/machine-learning/how-to-run-jupyter-notebooks?view=azureml-api-2)
