FROM ollama/ollama

WORKDIR /root

COPY . ./

#RUN apt update 
#RUN apt-get install -y python3 python3-pip vim git
#RUN pip install -r requirements.txt

ENTRYPOINT ["/root/entrypoint.sh"]