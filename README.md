# Neural Networks From Scratch

Projet personnel d'apprentissage du deep learning, construit progressivement
du neurone artificiel jusqu'aux réseaux de neurones profonds.

L'objectif principal est de comprendre les fondements mathématiques et
algorithmiques des réseaux de neurones tout en produisant des implémentations
lisibles, reproductibles et documentées.

## Objectifs

- Comprendre les composants d'un neurone artificiel
- Implementer la propagation avant
- Calculer et minimiser une fonction de coût
- Comprendre les gradients et la retropropagation
- Classifier des images avec NumPy
- Construire un réseau à deux couches
- Construire un réseau profond
- Comparer les implementations NumPy et PyTorch

## Progression

| Étape | Contenu | Statut |
|---|---|---|
| 1 | Neurone artificiel | Terminé |
| 2 | Classification d'images avec une couche | Terminé |
| 3 | Réseau de neurones à deux couches | À venir |
| 4 | Rétropropagation | À venir |
| 5 | Programmation du réseau à deux couches | À venir |
| 6 | Réseau de neurones profond | À venir |
| 7 | Implémentation avec PyTorch | À venir |

## Structure du projet

```text
neural-networks-from-scratch/
├── datasets/       # Jeux de données locaux
├── notebooks/      # Expériences et démonstrations
├── README.md
├── requirements.txt
└── .gitignore
```

## Contenu actuel

### Neurone artificiel

[first_neurone.ipynb](first_neurone.ipynb) présente :

- la génération de données binaires avec `make_blobs`
- l'initialisation des paramètres
- la fonction sigmoïde
- la log-loss
- le calcul des gradients
- la descente de gradient
- la frontière de décision
- une visualisation de l'espace des paramètres

### Classification d'images

[image_classification_one_layer_neuron.ipynb](image_classification_one_layer_neuron.ipynb)
présente :

- le chargement de données HDF5
- la conversion des images en vecteurs
- la normalisation des données
- l'entraînement d'un classificateur linéaire
- le suivi de la loss et de l'accuracy
- la comparaison des performances d'entraînement et de test

## Installation

Python 3.10 ou plus récent est recommandé.

```bash
git clone https://github.com/<utilisateur>/neural-networks-from-scratch.git
cd neural-networks-from-scratch

python -m venv .venv
source .venv/bin/activate       # Linux/macOS
# .venv\Scripts\activate        # Windows

python -m pip install --upgrade pip
python -m pip install -r requirements.txt
python -m ipykernel install --user --name neural-networks
```

Pour Windows PowerShell, l'environnement virtuel peut être activé avec :

```powershell
.venv\Scripts\Activate.ps1
```

## Utilisation

Ouvrir le projet dans Jupyter Notebook ou VS Code :

```bash
jupyter notebook
```

Sélectionner ensuite le kernel `neural-networks`, puis exécuter les notebooks
dans l'ordre.

## Jeux de données

Les fichiers contenus dans `datasets/` sont utilisés pour les notebooks
d'expérimentation actuels.

Avant toute réutilisation ou redistribution, vérifier séparément l'origine,
la licence et les conditions d'utilisation de chaque fichier. Les données
locales ne doivent pas être considérées comme publiquement redistribuables
sans confirmation explicite.

## Dépendances principales

- NumPy : calcul matriciel
- H5py : lecture des jeux de données au format HDF5
- Matplotlib : visualisations statistiques
- Plotly : visualisations interactives
- scikit-learn : données synthétiques et métriques
- tqdm : suivi de l'entraînement
- Jupyter : exécution des notebooks
- PyTorch : implémentation à venir

## Ressources visuelles

Le projet mettra progressivement en évidence :

- les frontières de décision ;
- les surfaces de fonction de coût ;
- les trajectoires d'optimisation ;
- les courbes d'entraînement et de validation ;
- les dimensions des tenseurs entre chaque couche ;
- les performances train/test.

## Objectif professionnel

Ce projet vise à construire une compréhension pratique du deep learning pour
préparer une candidature à un stage de recherche de six mois en intelligence
artificielle en France, en Belgique ou au Canada.

L'accent est placé sur :

- la compréhension des mathématiques ;
- l'implémentation à la main ;
- la reproductibilité ;
- la rigueur expérimentale ;
- la qualité du code ;
- la communication scientifique.

## Améliorations prévues

- extraction des fonctions dans des modules Python réutilisables
- séparation stricte train/validation/test
- seed globale pour la reproductibilité
- gradient checking
- mini-batch gradient descent
- initialisation He/Xavier
- régularisation L2
- dropout
- early stopping
- tests unitaires
- benchmark NumPy/PyTorch
- suivi des expériences
- comparaison de plusieurs architectures

## Licence

La licence du code n'est pas encore définie. Une licence MIT est envisagée,
mais elle ne sera ajoutée qu'après vérification des licences applicables aux
données et aux éléments de visualisation utilisés.
