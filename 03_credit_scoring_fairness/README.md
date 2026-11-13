# Audit et atténuation des biais algorithmiques dans le scoring de crédit

**Projet académique — AMSE, mai 2026**  
**Auteurs :** Loukmane BOULANKI et Céline ADOUSSINGANDE  
**Encadrant :** Pr Christophe Hurlin

## Question de recherche

Comment détecter et atténuer les disparités liées au genre dans les prédictions d'un modèle de scoring de crédit, tout en tenant compte à la fois de la performance prédictive et de l'incertitude statistique ?

## Données et modèles

L'étude utilise le jeu de données German Credit (1 000 observations) et compare trois modèles :
- régression logistique ;
- Random Forest ;
- LightGBM.

L'indicateur de groupe protégé est construit à partir des variables disponibles dans le jeu de données ; les limites de cette construction sont discutées dans le rapport.

## Méthodologie

- Analyse exploratoire et encodage des variables.
- Évaluation prédictive sur un échantillon d'entraînement et de test stratifié.
- Mesures d'équité fondées sur des seuils, dont le Disparate Impact.
- Test inférentiel d'équité suivant Hurlin et al. (2024).
- Utilisation de Fairness Partial Dependence Plots (FPDP) et neutralisation d'une variable au moment de la prédiction.

## Résultat principal

Pour Random Forest, le Disparate Impact est d'environ 0,88 et satisfait donc le seuil des quatre cinquièmes, tandis que le test inférentiel de parité statistique rejette l'hypothèse nulle au seuil de 5 % (F = 4,53 ; p = 0,033). La neutralisation de la variable *Payment Status of Previous Credit* à la modalité 2 conduit à F = 2,49 (p = 0,114), tandis que l'accuracy sur le jeu de test passe de 0,747 à 0,763 et l'AUC de 0,750 à 0,754.

## Limites

Le jeu de données est de petite taille et date de 1994. L'indicateur de groupe protégé combine des informations relatives au genre et à la situation matrimoniale. Enfin, la procédure d'atténuation étudiée porte sur une variable à la fois. Ces limites restreignent la portée de la généralisation et de l'interprétation des résultats.

## Ressources

- [Notebook Python sur Google Colab](https://colab.research.google.com/drive/17nu2eLE56w4oA1UsPMfo8DQKROF4DdMr?usp=sharing)
- Le rapport complet pourra être ajouté à ce dossier dans une version destinée à la diffusion publique.
