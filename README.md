Projet HNS - TopUrbi
Master 2 Humanités Numériques – École des Chartes – Janvier 2026
Autrice : Susanna De Luca
Contact : susanna.de.luca@chartes.psl.eu

Description générale du projet:
Ce projet s’inscrit dans le cadre du cours de Humanités Numériques Spatialisées et vise à analyser et cartographier les lieux mentionnés dans le dictionnaire TopUrbi (dictionnaire d’Alcedo). Le travail consiste à extraire les données du fichier XML de l’index TopUrbi, les structurer, géolocaliser les lieux et produire une série de cartes thématiques permettant d’explorer la distribution spatiale, la qualité de la localisation, les typologies des lieux et d’autres aspects interprétatifs.

L’ensemble du travail a été réalisé dans Google Colab en Python, avec l’utilisation des bibliothèques lxml, pandas, geopandas, matplotlib et shapely.

Données utilisées:
Le fichier principal traité est le fichier XML contenant l’index TopUrbi (TopUrbiIndex.xml).
Ce fichier inclut pour chaque lieu : un identifiant, les noms de lieu, des informations toponymiques structurées, des catégories de lieu, des indications sur la précision de la localisation, des coordonnées lorsque disponibles.

Les données ont été nettoyées, réorganisées et converties en GeoDataFrame pour permettre la cartographie.

Objectifs principaux:
1. extraire et structurer l’ensemble des lieux présents dans TopUrbi.
2. identifier et distinguer les lieux précisément localisés et ceux dont la localisation est approximative.
3. produire des cartes thématiques montrant: la distribution géographique générale, les différences entre lieux bien localisés et lieux approximatifs, les typologies des lieux, des zonages régionaux (découpage territorial), des comparaisons de densité, une analyse exploratoire complémentaire.
4. fournir des éléments d’interprétation utiles pour le mini-mémoire final.

Le notebook génère un total de neuf cartes :

1. Carte panoramique générale des lieux géolocalisés.
2. Carte des lieux précisément localisés.
3. Carte des lieux approximativement localisés.
4. Carte combinée bien localisés vs approximatifs.
5. Carte en découpage territorial (Caraïbes, Amérique centrale, Amérique du Nord, Andes, Cône Sud).
6. Carte des typologies de lieux (feature_type).
7. Carte des lieux avec coordonnées de type provincial_dummy.
8. Carte des macro-orientations géographiques (Nord/Sud, Est/Ouest).
9. Carte comparative de densité (well_placed vs provincial_dummy).

Dans sa structure le notebook contient: importation et vérification du fichier XML, extraction des données topographiques, traitement sémantique des catégories, transformation en GeoDataFrame, chargement du fond de carte Natural Earth, production des cartes thématiques, commentaires interprétatifs pour chaque carte.

Finalité du projet:
Le travail vise à produire une base cartographique cohérente permettant l’analyse spatiale du contenu du dictionnaire d’Alcedo. Les cartes obtenues serviront de support à une présentation orale et feront partie intégrante du mini-mémoire final, en fournissant des pistes d’interprétation sur la distribution géographique des lieux, la précision des localisations et les logiques sous-jacentes dans les sources historiques.
