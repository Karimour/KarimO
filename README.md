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
