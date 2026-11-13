# Bouygues Telecom — Ingénierie des données et analyse prédictive

**Étude de cas professionnelle** · Python · VBA · SQL · Docker · Streamlit · Modélisation prédictive

> Cette étude de cas présente mes contributions à un niveau général. Aucun code source interne, jeu de données de l'entreprise, indicateur confidentiel ou détail d'architecture propriétaire n'est publié.

## Vue d'ensemble

Mon expérience s'est articulée autour de deux volets complémentaires : la modernisation d'un processus existant de traitement des données et la mise à disposition des équipes métier d'un outil d'analyse prédictive des ventes.

## 1. Modernisation d'un processus de traitement initialement fondé sur VBA

### Contexte et compréhension de l'existant

À mon arrivée, j'ai repris un environnement de traitement reposant sur un ensemble de macros VBA. Avant d'engager la migration, j'ai dû comprendre le fonctionnement complet du processus en production : origine des données, étapes de transformation, circulation entre les différents traitements et usages des données par les applications et équipes en aval.

### Démarche et réalisations

- **Analyse de l'existant et cartographie des flux :** étude du fonctionnement des macros VBA, suivi des mouvements de données, des transformations, des dépendances et des usages en aval dans l'environnement de production.
- **Documentation technique :** formalisation du processus de bout en bout et modélisation des interactions et structures à l'aide de diagrammes UML de cas d'utilisation, de séquence et de classes.
- **Pilotage progressif :** construction d'une feuille de route pour organiser la migration par étapes, suivre l'avancement, recueillir les retours et faire valider les livrables au fur et à mesure.
- **Migration vers Python :** remplacement progressif des traitements VBA par une application Python connectée au Data Warehouse. L'application automatise les opérations ETL et fournit aux développeurs des données structurées dans les formats attendus.
- **Fiabilisation et exécution :** mise en place de tests de non-régression afin de vérifier la cohérence des traitements migrés, puis conteneurisation avec Docker pour faciliter le lancement de l'application par l'équipe.

### Compétences mobilisées

Compréhension d'un système existant · Cartographie des flux de données · Documentation technique · Modélisation UML · Livraison itérative · ETL Python · Tests de non-régression · Docker

## 2. Analyse prédictive des déterminants des ventes d'offres mobiles

### Problématique métier

Le second volet consistait à étudier les facteurs associés aux variations des volumes de ventes des offres mobiles et à fournir aux équipes métier un outil leur permettant d'explorer différentes hypothèses commerciales.

Une question étudiée, par exemple, était de savoir comment une variation du commissionnement versé aux partenaires pouvait être associée à une évolution des volumes de ventes.

### Démarche et réalisation

- Analyse des données commerciales afin d'étudier les déterminants associés aux évolutions des volumes de ventes des offres mobiles.
- Mise en place d'une démarche de modélisation prédictive pour explorer les relations entre les variables explicatives et les indicateurs commerciaux.
- Développement d'une interface Streamlit permettant aux utilisateurs métier de paramétrer leurs analyses, de sélectionner les KPI à examiner et de modifier les paramètres des scénarios.
- Possibilité de faire varier certaines hypothèses — notamment le niveau de commissionnement des partenaires — puis d'observer les variations correspondantes des volumes de ventes prédits et des indicateurs sélectionnés.

### Apport pour les équipes métier

L'interface rend l'analyse quantitative accessible à des utilisateurs non techniques. Sans avoir à manipuler le code ou les jeux de données, ils peuvent configurer leurs analyses, explorer des scénarios commerciaux et alimenter leurs réflexions à partir de résultats issus de la modélisation.

**Précaution d'interprétation :** les résultats des scénarios sont des prédictions conditionnelles aux hypothèses saisies dans le modèle. Ils ne constituent pas, à eux seuls, une preuve d'effet causal ; une telle conclusion nécessiterait une stratégie d'identification causale adaptée.

## Synthèse des compétences

| Domaine | Compétences |
|---|---|
| Ingénierie des données | Python, ETL, connexion au Data Warehouse, transformation des données |
| Conception et livraison | Migration VBA vers Python, UML, documentation technique, feuille de route, Docker |
| Qualité des données | Tests de non-régression, validation progressive |
| Data Science | Analyse exploratoire, modélisation prédictive, analyse de scénarios |
| Outils métier | Streamlit, paramétrage des KPI, aide à la décision |

## Confidentialité

Cette présentation ne contient volontairement aucune donnée interne, aucun code source propriétaire, aucune information client, aucun chiffre de performance confidentiel ni détail sensible de mise en œuvre. Elle vise à décrire la nature de mes contributions sans reproduire les systèmes internes de Bouygues Telecom.
