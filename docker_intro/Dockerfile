#PEGANDO DISTRIBUIÇÂO COM A IMAGEM
FROM python:slim

RUN pip3 install streamlit

#COPIANDO PARA O DOCKERFILE
COPY hello.py /src/
COPY web.py /src/

WORKDIR /src/

#DEFININDO QUE O ARQUIVO VAI SER EXECUTADO QUANDO A IMAGEM FOR RODADA SEM PARAMETROS
CMD ["streamlit","run","web.py","--server.address=0.0.0.0"]
