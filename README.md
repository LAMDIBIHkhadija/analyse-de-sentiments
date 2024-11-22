# **Analyse de Sentiments des Commentaires d'Hôtels**

Ce projet utilise le modèle pré-entraîné **RoBERTa** pour analyser les sentiments exprimés dans les commentaires d'utilisateurs sur les hôtels. Le modèle identifie si un commentaire reflète un sentiment **positif**, **neutre**, ou **négatif**. 

---

## **Objectif**

L'objectif de ce projet est de développer un système capable de classer les avis textuels en fonction de leur sentiment, en effectuant des étapes de prétraitement du texte, en appliquant le modèle **RoBERTa**, et en visualisant les résultats pour interpréter la répartition des sentiments.

---

## **Étapes principales**

1. **Importation du Jeu de Données**  
   - Chargement d'un fichier CSV contenant les avis textuels (`review_text`) soumis par les utilisateurs.  

2. **Préparation des Données**  
   - Nettoyage des données textuelles pour éliminer les informations inutiles :  
     - Conversion en minuscules.  
     - Suppression des balises HTML, URLs, ponctuation, nombres et accents.  
     - Élimination des stopwords et des emojis.  
     - Conversion des abréviations de chat en leur forme complète.  

3. **Analyse des Sentiments**  
   - Utilisation du modèle pré-entraîné **`cardiffnlp/twitter-roberta-base-sentiment-latest`** via la bibliothèque **HuggingFace Transformers** :  
     - Chaque commentaire est classé dans l'une des catégories suivantes : **positif**, **neutre**, ou **négatif**.  

4. **Visualisation des Résultats**  
   - Génération de graphiques pour représenter la distribution des sentiments sur l'ensemble des commentaires.  

---

## **Jeu de Données**

Le jeu de données utilisé pour ce projet peut être téléchargé depuis le lien suivant :  
- [Lien vers le dataset](https://www.kaggle.com/datasets/thedevastator/booking-com-hotel-reviews)

---

## **Auteur**

- [Khadija Lamdibih](https://github.com/LAMDIBIHkhadija) 
