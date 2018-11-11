# Answers

Nom: Magadis
Prénom: Aïda 
NB: 7

## 1.3
command: docker run -it --rm --name my-running-app my-python-app

## 1.4
answer: L'adresse ne répond rien car il y a une erreur concernant la variable d'environnement.
command : docker run -it --rm --name my-running-app -p 8080:8080 my-python-app 

## 1.5
command: docker run -it -e ENVIRONMENT='dev' --rm --name my-running-app -p 8080:8080 my-python-app 

## 1.6
answer: L'image n'est pas censée se pousser car il faut mettre un tag avant de push.
command: 

## 1.7
answer: Avant que l'image ne démarre, celle-ci n'est pas trouvée localement (c'est parce qu'on l'a supprimée précédemment).
command: docker rmi -f f91a08a762a9
command: docker run -it -e ENVIRONMENT='dev' --rm --name my-running-app -p 8080:8080 aidamaga/my-python-app
command: docker run -it -d -e ENVIRONMENT='dev' --rm --name my-running-app -p 8080:8080 aidamaga/my-python-app

## 1.8
answer: En tapant la commande "docker ps" on aperçoit différentes colonnes dont NAMES qui indique le nom du container (ici "my-running-app") et STATUS qui indique si le container est en cours d'exécution ou pas (ici "Up About a minute" donc le container est bien démarré). 
command: docker ps
command: docker rename my-running-app my-container

## 1.9
answer: L'OS utilisé dans le container est debian.
answer:
DISTRIB_ID=Ubuntu
DISTRIB_RELEASE=18.04
DISTRIB_CODENAME=bionic
DISTRIB_DESCRIPTION="Ubuntu 18.04.1 LTS"
NAME="Ubuntu"
VERSION="18.04.1 LTS (Bionic Beaver)"
ID=ubuntu
ID_LIKE=debian
PRETTY_NAME="Ubuntu 18.04.1 LTS"
VERSION_ID="18.04"
HOME_URL="https://www.ubuntu.com/"
SUPPORT_URL="https://help.ubuntu.com/"
BUG_REPORT_URL="https://bugs.launchpad.net/ubuntu/"
PRIVACY_POLICY_URL="https://www.ubuntu.com/legal/terms-and-policies/privacy-policy"
VERSION_CODENAME=bionic
UBUNTU_CODENAME=bionic

## 1.11
command: 

## 2.1
command: 

## 2.6
command: 
command: 


