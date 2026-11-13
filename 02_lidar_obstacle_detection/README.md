# Airbus AI Hackathon 2026 — Détection d'obstacles par LiDAR 3D

**Thème :** perception 3D à partir de nuages de points LiDAR pour la sécurité des vols à basse altitude.

## Problématique

Le challenge porte sur la détection d'obstacles susceptibles de présenter un risque pour les vols d'hélicoptères à basse altitude : antennes, câbles électriques, poteaux et éoliennes. Les données d'entrée sont des nuages de points LiDAR simulés, comportant des informations de classification au niveau des points.

## Approche du projet

Les travaux présentés dans mon CV comprennent :
- une approche de détection 3D fondée sur PointPillars++ ;
- la reconstruction de boîtes de vérité terrain (*ground-truth boxes*) à l'aide de DBSCAN et de l'analyse en composantes principales (PCA) ;
- l'utilisation de PyTorch et Open3D pour la modélisation et le traitement des nuages de points.

Cette présentation décrit le périmètre des travaux ; elle ne remplace pas le code source ni un benchmark expérimental complet.

## Technologies et méthodes

Python · PyTorch · Open3D · Nuages de points · PointPillars++ · DBSCAN · PCA

## Ressources et reproductibilité

Le notebook, les scripts, les configurations et les éventuelles visualisations autorisées ne sont pas disponibles dans ce dépôt à ce stade. Aucune donnée du challenge ni aucun contenu à diffusion restreinte n'est publié ici.
