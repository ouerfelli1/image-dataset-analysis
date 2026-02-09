# image-dataset-analysis
# Titre du projet : Classfication des images médicales 

## Objectif
Une application web basée sur un modèle CNN capable de classifier automatiquement des images de lésions cutanées pour distinguer différents types de cancer de la peau (et lésions bénignes) à partir du dataset HAM10000

## Dataset
- Nom du dataset : Skin Cancer MNIST: HAM10000
- Lien du dataset : https://www.kaggle.com/datasets/kmader/skin-cancer-mnist-ham10000

## Équipe
- OUERFELLI Oumaima

## Exploration du dataset
Cette section présente une analyse descriptive du dataset d’images HAM10000, un jeu de données couramment utilisé en dermatologie pour la classification automatique de lésions cutanées.
Le dataset contient des images dermatoscopiques représentant différents types de lésions cutanées bénignes et malignes.

### Nombre d’images par classe
Nom du dataset : Skin Cancer MNIST: HAM10000
Total d’images : 10 015 images dermatoscopiques.
Format des images : JPEG
Nombre de classes : 7 catégories diagnostiques de lésions cutanées

### Observations
*Déséquilibre important :
La classe nv représente près des deux tiers du dataset, tandis que certaines classes comme df ou vasc sont fortement sous-représentées. Ce déséquilibre peut influencer l’apprentissage des modèles, qui auront tendance à être biaisés vers les classes majoritaires.
*Impli­ca­tions pour l’entraînement :
Le déséquilibre appelle à utiliser des techniques telles que :
1/ la data augmentation des classes rares
2/ la pondération par classes dans la fonction de perte
3/ le resampling des données pour équilibrer les classes
*Diversité des lésions :
Les images couvrent un large spectre de conditions dermatologiques, des lésions bénignes aux cancers agressifs, ce qui rend le dataset pertinent pour des tâches de classification multiclasses.

## Architecture du projet
- Back-end : Python / FastAPI / API REST
- Front-end : React.js / Type Script / Axios / Material UI
- Données : images
- Visualisation : Dashboard
![Architecture](architecture.PNG)
