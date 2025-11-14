# Introduction au Prompt Engineering

Support de présentation pour Naela - Stage 3ème

## Description

Cette présentation Quarto/R introduit les concepts de base du Prompt Engineering pour un public de collégiens (3ème). Elle est déployée automatiquement sur GitHub Pages.

## Structure du projet

```
stage_troisieme/
├── index.qmd              # Présentation principale (Quarto Markdown)
├── _quarto.yml            # Configuration du projet Quarto
├── custom.scss            # Styles personnalisés (SCSS)
├── styles.css             # Styles CSS additionnels
├── images/                # Dossier pour les images et le logo
├── .github/workflows/     # GitHub Actions pour le déploiement
└── docs/                  # Dossier de sortie (généré, déployé sur GitHub Pages)
```

## Prérequis

Pour travailler en local sur cette présentation, vous aurez besoin de :

- [Quarto](https://quarto.org/docs/get-started/) (version 1.4 ou supérieure)
- [R](https://www.r-project.org/) (version 4.3 ou supérieure)
- Packages R : `rmarkdown`, `knitr`

## Installation locale

1. Cloner le dépôt :
```bash
git clone https://github.com/MaryleneH/stage_troisieme.git
cd stage_troisieme
```

2. Installer les dépendances R :
```r
install.packages(c("rmarkdown", "knitr"))
```

## Générer la présentation

### En ligne de commande

```bash
quarto render
```

Cette commande génère la présentation dans le dossier `docs/`.

### Prévisualiser en local

```bash
quarto preview
```

Cela ouvre un serveur local avec rechargement automatique.

## Déploiement sur GitHub Pages

Le déploiement est automatique via GitHub Actions :

1. Chaque commit sur la branche `main` déclenche le workflow
2. Quarto génère la présentation dans le dossier `docs/`
3. Le contenu est déployé automatiquement sur GitHub Pages

### Configuration de GitHub Pages

Dans les paramètres du dépôt GitHub :
- Aller dans **Settings** > **Pages**
- Source : **GitHub Actions**

L'URL de la présentation sera : `https://maryleneh.github.io/stage_troisieme/`

## Personnalisation

### Modifier le contenu

Éditez le fichier `index.qmd` pour modifier le contenu de la présentation.

### Modifier les styles

- `custom.scss` : styles SCSS pour le thème Reveal.js
- `styles.css` : styles CSS additionnels

### Ajouter des images

Placez vos images dans le dossier `images/` et référencez-les dans `index.qmd` :

```markdown
![Description](images/mon-image.png)
```

### Ajouter un logo

Remplacez `images/logo.png` par votre logo (taille recommandée : 200x200 pixels).

## Structure de la présentation

La présentation couvre les sujets suivants :

1. Introduction au Prompt Engineering
2. Qu'est-ce qu'un prompt ?
3. Pourquoi le Prompt Engineering ?
4. Principes de base
5. Exemples pratiques
6. Techniques avancées
7. Exercice pratique
8. Erreurs à éviter
9. Ressources et outils
10. Conclusion

## Contribuer

Pour contribuer à cette présentation :

1. Créez une branche : `git checkout -b ma-modification`
2. Faites vos modifications
3. Commitez : `git commit -am 'Description de la modification'`
4. Poussez : `git push origin ma-modification`
5. Créez une Pull Request

## Licence

Ce projet est un support éducatif pour un stage de 3ème.
