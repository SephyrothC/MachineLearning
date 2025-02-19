# Decider sans apprendre

## Décider SANS apprendre : plus proche voisin

* **Données de départ** :
  Un ensemble d’exemples de référence E de vecteurs étiquetés Xi avec ydi la classe associée
* **Objectif** :
  Décider de la classe d’un vecteur inconnu X
* **Méthode** :
  Calculer les distances entre X et l’ensemble des vecteurs Xi de E
  Attribuer à X la classe de son plus proche voisin (distance minimum)

## Extension : k-plus-proches-voisins

1. Calculer la distance entre X et tous les exemples de la base de référence
2. Déterminer les k vecteurs PPV(X) de la base les plus proches
    * **k = 1** : Ci = argmin d(Xi, X)
    * **k ≠ 1** : Ci = classe majoritaire de {PPV(X)}
    * **Variante** : unanimité sinon rejet, prise en compte de la distance

## Calcul de distance (variables quantitatives)

![image_2.png](image_2.png)

distance euclidienne (norme L2) : $$ d(X_1, X_2) = \sqrt{\sum_{i=1}^{i=D} (x_{1i} - x_2i)^2} $$



## Dilemme biais-variance

![image_3.png](image_3.png)

## L’algorithme parfait ?
Avantages :
* Très simple à mettre en œuvre (lazy learning)
* Naturellement multiclasse
* Incrémental
* Tend asymptotiquement (N→∞) vers l’erreur optimale $$ ε_{B} < ε_{ppv} < 2ε_{B} $$
* S’adapte facilement à la régression : $$ y = \frac{1}{k} \sum_{i=1}^{k} y_{di} $$

## Bilan
Algorithme « baseline » pour évaluer la complexité d’un problème, la qualité des données…

- Accélérateurs : diminuer D ou N (module datamining)
    - réduction de dimension
    - catégorisation (clustering)

