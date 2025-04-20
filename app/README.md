###### important - Current docker version does not work, need to execute it Locally ######

Install ollama server from - https://ollama.com/download/windows

once installed use command - ollama -help

Start ollama service if not alread y -ollama serve &

pull latest llm model - ollama pull llama3

create virtual environment - python -m venv .langchain

activate virtual environment - .langchain\Scripts\activate

Install Dependencies - pip install -r requirements.txt

run streamlit app - streamlit run app/main.py --server.port=8501 --server.address=0.0.0.0

Open browser and redirect to - http://localhost:8501