FROM ubuntu

RUN apt-get update && apt-get install -y python pip git
RUN pip install virtualenv
COPY ../src/run.sh ~/run.sh

EXPOSE 80

CMD git clone https://github.com/owlbread/LSTM-docker-service.git && cd LSTM-docker-service/src && ./run.sh
