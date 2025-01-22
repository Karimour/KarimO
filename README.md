# KarimO
Mardi: Contribution à l'excercice en nettoyant un jeu de donnes en rapport avec notre porjet et en utilisant un outil de visiualiation nommée Data wrapper, les roblèmes rencontrés : Type de graphique inadéquat : Datawrapper essayait de créer un graphique linéaire, mais les données ne contenaient pas de colonne numérique pour l'axe vertical, seulement des codes (texte) et des années (date).
Format de données incorrect: Datawrapper n'a pas pu reconnaître ou utiliser correctement les données importées car les colonnes n'étaient pas correctement identifiées comme du texte, des nombres ou des dates. 

Les Solutions :
Choisir le bon type de graphique : Sélectionner une "Grouped Colomuns" au lieu d'un graphique linéaire, car ce type de carte est adapté pour visualiser ses données de comparaison 
Nettoyer et formater les données :
Manuellement supprimer les lignes et colonnes superflues : Enlever les lignes inutiles du fichier CSV.
Définir les types de données : Dans l'étape "Check & Describe" de Datawrapper, vérifier et corriger le type de chaque colonne : "Text" pour les pays, "Date" pour les années et s'assurer d'avoir une colonne de type "Number" avec les valeurs à visualiser.

Liens pour le Datavis Atelier Mercredi:
https://api.npoint.io/f671ae05239dd566d68f

Eg. Visualisation pour le projet : Catégorie,Île-de-France (Numérique),Île-de-France (Économie totale),Province (Numérique),Province (Économie totale)
Part des femmes,23.6,48.5,20.3,48.4
Part des <35 ans,41.8,32.8,38.9,30.4
Part des cadres,76.4,30.1,57.8,14.5
Résultat: 
https://www.datawrapper.de/_/1tjd4/

1. Une première visualisation doit contenir des données structurées. Votre visualisation doit être interactive est accessible sur GitHub Pages:
Visualisation interactive : https://karimour.github.io/KarimO/ - https://github.com/Karimour/KarimO/commit/c64b2a02ce3a11404878231e4f2f0ee0ed626698#diff-ec6513e5a78c1848d5b285250332c930f40d3afe7b8701ed831149f38906a980
![Image 22-01-2025 at 14 20](https://github.com/user-attachments/assets/0b2cd51c-6242-4b84-84d4-ea7c5db98b86)

2eme exemple : Répartition par sexe des familles professionnelles et des principales professions du numérique en 2021-2022
![nDZLV-r-partition-par-sexe-des-familles-professionnelles-et-des-principales-professions-du-num-rique-en-2021-2022-2](https://github.com/user-attachments/assets/0c631154-cbf6-44c5-b86d-12e46aaf8ecf)
<div style="min-height:673px" id="datawrapper-vis-nDZLV"><script type="text/javascript" defer src="https://datawrapper.dwcdn.net/nDZLV/embed.js" charset="utf-8" data-target="#datawrapper-vis-nDZLV"></script><noscript><img src="https://datawrapper.dwcdn.net/nDZLV/full.png" alt="" /></noscript></div>


Données non-structurées. Cette visualisation peut être interactive mais aussi statique avec des annotations et légendes sur la visualisation elle-même.
Nuage de mots: 



