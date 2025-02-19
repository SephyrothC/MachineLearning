# Introduction

## Applications en aide à la décision : exemples et principes
### Qu’est-ce qu’être intelligent ?
#### Savoir Apprendre
- élaborer un système de connaissances **à partir des données**
- pouvoir **intégrer de nouvelles données** (connaissances)
- _supervisé_ (par un professeur) ou _non supervisé_ (par association)
#### Savoir Raisonner (déduire, anticiper)
- à partir du système de connaissances **et des données** de l’expérience pouvoir
produire
  - Une décision
  - de nouvelles connaissances

### Qu’est-ce que le machine learning ?
- C'est une voix dans l'intelligence artificielle qui consiste a généré des modèles à partir de données réelles. 
- Construire un model à partir d'observations.


## Données et bases de données

### Bases de données
Matrice de données : D*N (#Dimensions * #Exemples)

| X1  | X2  | X3  | ... | XN  |
|-----|-----|-----|-----|-----|
| x11 | x21 | x31 | ... | xN1 |
| x12 | x22 | x32 | ... | xN2 |
| ... | ... | ... | ... | ... |
| x1D | x2D | x3D | ... | xND |

Signification:

| y1  | y2  | y3  | ... | yN  |
|-----|-----|-----|-----|-----|

## Classification ou régression ?

### Formalisation
**Exemple = Observation + Signification** → apprentissage supervisé

**Observation** : vecteur aléatoire Xj=(x1, x2,… xD)
- xi : caractéristiques, descripteurs, features, variables explicatives
    - Qualitatives (nominales / ordinales)
    - Quantitatives (continues / discrètes)
- D : dimension de l’espace de représentation

**Signification** : ydj
- ydi ∈ ℝ : variable quantitative → **régression** variable à expliquer/prédire
- ydi ∈ ℕ : variable qualitative → **classification** vérité terrain, label, classe
- K : dimension de l’espace de décision (== nombre de classes)
  → **Fonction de classification** : soit X l’espace des entrées (représentation) et Y, celui des sorties (décision)

**h : X → Y tell    e que h(Xj) ≈ ydj**

