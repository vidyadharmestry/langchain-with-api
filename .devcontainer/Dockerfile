FROM python:3.9-slim

WORKDIR /app

COPY ../../streamlit/requirements.txt .
#COPY ../streamlit/streamlit_app.py .


RUN apt-get update && apt-get install -y \
    build-essential \
    curl \
    software-properties-common \
    git \
    && rm -rf /var/lib/apt/lists/*

#RUN git clone https://github.com/streamlit/streamlit-example.git .

RUN pip install --upgrade pip

RUN pip3 install -r ../streamlit/requirements.txt

EXPOSE 8501

HEALTHCHECK CMD curl --fail http://localhost:8501/_stcore/health

ENTRYPOINT ["streamlit", "run", "streamlit_app.py", "--server.port=8501", "--server.address=0.0.0.0"]