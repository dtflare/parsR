This is a work in progress, current version works great for scraping / parsing text content from xml websites.

This was built using Linux Ubuntu, please adjust the below directions per your OS.

Create a new Miniconda environment, & apply the following settings:
$ conda create --name myenv python=3.8
$ pip install langchain==0.1.4 deeplake openai==1.10.0 tiktoken

Launch Langchain's newspaper module:
$ !pip install -q newspaper3k python-dotenv

Export your OpenAI API Key within your Miniconda environment - will expire when session ends.
$ export OPENAI_API_KEY=<>

Adjust script as needed, currently it will output OPENAI's JSON format for Fine-Tuning.

Assign execute permissions
$ chmod +x parsR

Add parsR to $PATH, either in your .bashrc file, or include it within a file in your $PATH
OR 
simply run with ./

To run parsR once added to your global path:
$ parsR website_url.com file_name.json


