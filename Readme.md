## .env  -- file cannot be uploaded


<span style="color:#85c7f2"><strong>But it must be created inside the project (whether openai model is used or not)</strong></span>

**This is the example how it can be added**

```
OPENAI_API_KEY = "sk-proj-111..."
```


## virtual environment must be created 


<span style="color:#85c7f2"><strong>Either use conda environment or make venv using python</strong></span>


```
conda create -p myenv python==3.12
```
or
```
python -m venv myenv
```


## Now install required packages in this environment
```
pip install crewai crewai-tools python-dotenv langchain_openai
```

<span style="color:#85c7f2"><strong>In order to use ollama models, install ollama in your system and then pull the desired model</strong></span>

```
ollama pull llama3.2
```

## Lastly run the main.py (the file in which all the crews are binded together) file
```
python main.py
```