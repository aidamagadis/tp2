FROM python:3.7.1-stretch

WORKDIR /Documents/Micro-Services/tp2/app


COPY requirements.txt ./
RUN pip install --no-cache-dir -r requirements.txt

COPY . .

CMD [ "python", "-u", "./webservice.py" ]
