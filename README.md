# Scoring_Linux
Projet réalisé avec [Yasmine Ouyahya](https://github.com/youyahya) et [Amira Slimene](https://github.com/aslimene).

Le but de ce projet est de réaliser une grille de score permettant d'aider à la décision.

Ainsi, on a créé une grille de score calibrée sur 1000 points, plus le score est élevé, moins le client a de risque de faire défaut. On fixe les Odds à 500:1 et les PDO (Points Double the Odds) à 30 points. 

Une personne qui a un  score 1000 points  a une probabilité de défaut de 1/500 alors qu'une personne qui a un score de 1030 (1000 + 30) elle a une une probabilité de défaut égale à 1000:1 = 2*500:1.

Pour la réalisation de ce projet, nous nous sommes inspirés d'un projet fait par [Carl Lejerskar](https://github.com/Carl-Lejerskar). Son projet est trouvable dans le dossier ***RepoInitial*** ou directement [ici](https://github.com/Carl-Lejerskar/HMEQ). Des améliorations et de nouvelles fonctionnalités ont été apportées et se trouvent dans le dossier ***Ameliorations***. 

Ce répertoire est divisé en 2 dossiers l'un contenant les données et l'autre les programmes nommés selon leurs fonctions.

On a créé un outil automatisé permettant selon les caractéristiques entrées de générer le score ainsi que la probabilité de défaut d'un emprunteur. Il est accessible ici [![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://share.streamlit.io/aadmberrada/linux_hmeq/main/app.py)

## Demo de l'application

Voici une petite démonstration de l'application créée :

![Example of Streamlit|635x680](https://raw.githubusercontent.com/aadmberrada/Linux_HMEQ/main/Ameliorations/2_Data/Demo_streamlit.gif)


## Usage
 - Prerequis
 ```pip install -r requirements.txt```
```py
    pandas==1.3.5
    streamlit==1.4.0
    sklearn
    scorecardpy 
```
 - App Web 
 ```streamlit run app.py```