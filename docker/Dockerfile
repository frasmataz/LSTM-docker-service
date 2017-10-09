FROM ubuntu

RUN apt-get update && apt-get install -y python pip git
RUN git clone https://github.com/owlbread/LSTM-docker-service.git
RUN cd LSTM-docker-service/src
RUN pip install virtualenv
RUN virtualenv -p python2.7 venv && source venv/bin/activate
RUN pip install -r requirements.txt

EXPOSE 80

CMD python __main__.py
