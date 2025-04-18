redirect to - ./streamlit

build docker - docker build -t streamlit .

Run Docker - docker run -p 8501:8501 streamlit

debug linux image - docker run -it --rm --entrypoint sh streamlit