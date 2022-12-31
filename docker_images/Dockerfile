FROM ubuntu

RUN apt-get update && apt-get -y install python3-pip
RUN pip3 install flask flask-mysql
COPY ./app.py /opt/source-code/app.py
#ENTRYPOINT FLASK_APP=/opt/source-code/app.py flask run
ENV FLASK_APP=/opt/source-code/app.py
CMD [ "python3", "-m" , "flask", "run", "--host", "0.0.0.0"]