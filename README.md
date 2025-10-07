# Créer un pipeline de modèle d'apprentissage automatique
Ce projet illustre la création d'un modèle de prevision en utilisant sklearn et l'algorithme de recherche
d'hyperparamètres optuna

# Données utilisées
Les données utilisées pour ce démonstrateur ont été générées par simulation numérique.
Elles représentent la puissance électrique d'une presse à balle (utilisée par exemple pour la compression de déchet sortants d'un salle de tri)
utilisée pour comprimer une couche de matière

Les variables sont les suivantes:

- *baler_power_kw*: puissance électrique de la presse à balle
- *ball_tick_before*: épaisseur de la matière avant compression
- *ball_tick_after*: épaisseur de la matière après compression
- *ball_area*: surface de la matière
- *material*: type de matière

la variable *material* est une variable catégorielle

# Modèle utilisé
Dans ce démonstrateur, j'utilise la librairie lightgmb qui, par expérience, m'a montrée de bonnes performances pour les modèles de regression
J'ai volontairement omis les statistiques descriptives car les outliers ont été supprimés préalablement

# Enregistrement du modèle
Je montre comment enregistrer le modèle au format onnx car c'est un format que j'ai souvent utilisé en production
