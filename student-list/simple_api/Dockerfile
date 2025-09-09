FROM python:3.11-slim
LABEL maintainer="Loic" email="loicpierret@live.fr"
COPY requirements.txt student_age.py /
RUN apt update -y && apt install python3-dev libsasl2-dev libldap2-dev libssl-dev gcc build-essential -y
RUN pip3 install -r /requirements.txt
VOLUME [ "/data" ]
EXPOSE 5000
CMD [ "python3", "./student_age.py" ]