# Answers

Nom: Magadis
Prénom: Aïda 
NB: 7

## 1.3
command: 
docker build -t my-python-app ./
docker run --name my-running-app my-python-app

## 1.4
answer: L'adresse ne répond rien car il y a une erreur concernant la variable d'environnement.
command : docker run --name my-running-app -p 8080:8080 my-python-app 

## 1.5
command: docker run -e ENVIRONMENT='dev' --rm --name my-running-app -p 8080:8080 my-python-app 

## 1.6
answer: L'image n'est pas censée se pousser car il faut mettre un tag avant de push.
command: docker tag my-python-app aidamaga/my-python-app

## 1.7
answer: Avant que l'image ne démarre, celle-ci n'est pas trouvée localement (c'est parce qu'on l'a supprimée précédemment).
command: docker rmi -f f91a08a762a9
command: docker run -e ENVIRONMENT='dev' --name my-running-app -p 8080:8080 aidamaga/my-python-app
command: docker run -d -e ENVIRONMENT='dev' --name my-running-app -p 8080:8080 aidamaga/my-python-app

## 1.8
answer: En tapant la commande "docker ps" on aperçoit différentes colonnes dont NAMES qui indique le nom du container (ici "my-running-app") et STATUS qui indique si le container est en cours d'exécution ou pas (ici "Up About a minute" donc le container est bien démarré). 
command: docker ps
command: docker rename my-running-app my-container

## 1.9
answer: L'OS utilisé dans le container est debian.
answer:
PRETTY_NAME="Debian GNU/Linux 9 (stretch)"
NAME="Debian GNU/Linux"
VERSION_ID="9"
VERSION="9 (stretch)"
ID=debian
HOME_URL="https://www.debian.org/"
SUPPORT_URL="https://www.debian.org/support"
BUG_REPORT_URL="https://bugs.debian.org/"
root@943b8b42b79f:/Documents/Micro-Services/tp2/app# 

## 1.11
command: docker run -e APP_PORT=8081 -e WS_BACK_URL=172.17.0.1 -p 8081:8081 aidamaga/my-python-app-front
answer : 
You called at : 2018-11-12 13:58:23.179888 (dynamic)
        On environment : dev (from env variable)
        With path : Here is the root   (from URL path)
        With front : 9e5b2fc98f51 (from real hostname of front service)
        With back  : 943b8b42b79f (from real hostname of back service)
        

## 2.1
command: docker-compose up

## 2.6
command: docker-compose up -d
command: docker-compose logs


