Au final, on veut:
  - Un readme
  - MIT
  - Donnée
  - Scripts/EDA
  - Présentation

Groupe 13

Modélisation spatiotemporelle prédictive du risque d'agression à Chicago 

0. Contexte 
Dans le cadre de ce projet, nous souhaitons développer un modèle capable de prédire la probabilité de crimes selon leur nature, leur localisation et leur temporalité sur la base du dataset des crimes à Chicago.
Etapes : préparation de données, analyses statistiques, modélisation prédictive et visualisation.
L’étude intégrera également une réflexion plus globale sur les éventuelles limites ou dérives, notamment la présence de biais algorithmiques.
Problématique
Comment construire un modèle fiable et interprétable pour prédire la survenue de crimes à Chicago à partir des données publiques disponibles ?
Sous-questions :
Quelles sont les tendances temporelles des crimes (heures, jours, saisons) ?
Quels sont les patterns spatiaux (quartiers, zones chaudes) ?
Quels types de features permettent d’améliorer l’efficacité du modèle prédictif ?
Quels algorithmes sont les plus adaptés à ce type de données (régression, arbres, modèles spatiaux) ?
Quelles sont les principales limites des prédictions ?
Une réflexion additionnelle portera sur la question :
Dans quelle mesure les données ou les algorithmes peuvent-ils être biaisés, et quels en seraient les effets ?
2. Objectifs et enjeux (SMART)
Objectif général :
Développer un pipeline complet de data science permettant d’explorer, préparer, analyser et modéliser les données criminelles de Chicago.

Objectifs SMART
Spécifique :
 Construire un ou plusieurs modèles prédictifs (régression logistique, random forest, modèles spatio-temporels) pour identifier les zones/temps à risque.


Mesurable :
 Évaluer les performances avec des métriques claires : accuracy, AUC, précision, rappel, matrice de confusion, validation croisée.
Atteignable :
 Utiliser des bibliothèques Python accessibles : pandas, scikit-learn, geopandas, matplotlib, folium.
Réaliste :
 Limiter l’étude à un périmètre donné :
une sélection de types de crimes (ex. vol, agression), ou
une période récente (2018–2023), ou
une échelle spatiale fixée (quartiers, grille)
Temporel :
 Réalisation sur X semaines avec jalons : EDA → feature engineering → modélisation → évaluation → ouverture sur les biais → rédaction.
3. Périmètre et limites
Périmètre du projet:
Utilisation des données publiques “Crimes – 2001 to Present".
Analyse statistique :
  Répartition temporelle des crimes / Cartographie des zones de concentration / Évolution de certains types de crimes


Construction d’un modèle prédictif.


Comparaison de plusieurs algorithmes.


Discussion sur les limites des données et des prédictions.


Ouverture : analyse de biais potentiels ou détection de distorsions dans les données.


⚠️ Limites:
Les données représentent des crimes enregistrés, non la criminalité réelle → distorsion possible.
Certaines variables clés (surveillance policière, population quotidienne réelle) ne sont pas incluses.
Le modèle ne peut pas prédire individuellement où un crime va se produire, mais seulement estimer des tendances.
L’étude des biais restera limitée (ouverture, non cœur du projet).



4. Mise en œuvre et réalisation
Étape 1 – Collecte et préparation des données
Nettoyage 
Agrégation ou création de features (jour de la semaine, saison, clusters spatiaux, etc.).
Étape 2 – Analyse exploratoire (EDA)
Statistiques descriptives.
Visualisation des cycles temporels (heures, jours, saisons).
Cartographie (zones chaudes, densité, clusters).
Identification de patterns exploitables


Étape 3 – Feature engineering
Construction de variables spatio-temporelles
Découpage de la ville en grilles / quartiers.
Création d’indicateurs locaux.


Étape 4 – Modélisation
Sélection d’un ou plusieurs modèles :

régression logistique,
random forest,
gradient boosting,
modèles spatio-temporels (optionnel).


Entraînement et validation croisée.
Mesure de performance.
Étape 5 – Analyse des résultats
Interprétation des performances.
Importance des variables.
Comparaison des modèles.
Visualisation des zones ou périodes prédites comme "à risque".


Étape 6 – Ouverture : limites et biais
Discussion sur les limites des données criminelles.
Mise en lumière de potentiels biais (surreprésentation de certaines zones, variables proxies).
Option : test rapide d'une technique simple de rééquilibrage spatial pour illustrer l’idée.
Illustration de comment ces biais pourraient affecter les prédictions.
Étape 7 – Conclusion et perspectives
Synthèse des résultats.
Évaluation de la pertinence des modèles.
Suggestions d’améliorations :
 → modélisation plus fine,
 → ajout de données externes,
 → analyse de biais plus poussée.
