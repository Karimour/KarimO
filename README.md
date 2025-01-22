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

Visualisation pour le projet : Catégorie,Île-de-France (Numérique),Île-de-France (Économie totale),Province (Numérique),Province (Économie totale)
Part des femmes,23.6,48.5,20.3,48.4
Part des <35 ans,41.8,32.8,38.9,30.4
Part des cadres,76.4,30.1,57.8,14.5
Résultat: 
https://www.datawrapper.de/_/1tjd4/

Année,Part des femmes (Ingénieurs),Part des femmes (Chefs de projet),Part des femmes (Total numérique)
2007,22.5,19.6,22.5
2016,24.2,25.1,23.6
Résultat: 
https://www.datawrapper.de/_/vT5Xx/

Dynamic Visualisation : https://github.com/Karimour/KarimO/commit/c64b2a02ce3a11404878231e4f2f0ee0ed626698#diff-ec6513e5a78c1848d5b285250332c930f40d3afe7b8701ed831149f38906a980
