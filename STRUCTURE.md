# Structure de la présentation - Référence rapide

## Vue d'ensemble

Cette présentation Quarto est organisée en diapositives thématiques sur le Prompt Engineering.

## Structure actuelle (index.qmd)

### 1. Page de titre
- Titre : "Introduction au Prompt Engineering"
- Sous-titre : "Apprendre à communiquer avec l'IA"
- Auteur : Stage 3ème

### 2. Bienvenue (slide d'introduction)
- Introduction au sujet
- Notes pour l'orateur

### 3. Qu'est-ce qu'un Prompt ?
- Définition du prompt
- Points progressifs (incremental)
- Concept de base

### 4. Pourquoi le Prompt Engineering ?
- Deux colonnes : Avantages / Applications
- Liste des bénéfices

### 5. Les Principes de Base
- Liste numérotée
- 3 principes fondamentaux

### 6. Exemples Pratiques
- Panneaux à onglets (tabset)
- 2 exemples avant/après

### 7. Techniques Avancées
- 4 techniques principales
- Points progressifs

### 8. Exercice Pratique
- Exercice interactif
- Solution en fragment

### 9. Erreurs à Éviter
- Liste d'erreurs courantes
- Bonnes pratiques

### 10. Ressources et Outils
- Liste de ressources
- Callout tip (astuce)

### 11. Conclusion
- Points clés
- Points progressifs
- Appel à questions

### 12. Merci
- Slide de remerciement
- Notes pour Q&A

## Éléments Quarto utilisés

### Classes CSS personnalisées
- `.center` : Centrer le contenu
- `.smaller` : Réduire la taille du texte
- `.incremental` : Affichage progressif
- `.fragment` : Fragment apparaissant au clic

### Composants Quarto
- `{.notes}` : Notes pour le présentateur
- `{.columns}` et `{.column}` : Mise en page multi-colonnes
- `{.panel-tabset}` : Panneaux à onglets
- `{.callout-tip}` : Boîte d'astuce

### Formatage
- `**texte**` : Texte en gras
- Liste numérotée : 1., 2., 3.
- Liste à puces : - item
- Émojis : 🤔, ❌, ✅

## Personnalisation facile

### Ajouter une nouvelle slide

```markdown
## Titre de la slide {.center}

Contenu de la slide

::: {.notes}
Notes pour le présentateur
:::
```

### Ajouter une image

```markdown
![Description de l'image](images/nom-image.png)
```

### Ajouter une vidéo

```markdown
{{< video https://www.youtube.com/watch?v=VIDEO_ID >}}
```

### Ajouter du code

````markdown
```python
# Code Python
print("Hello, Prompt Engineering!")
```
````

### Ajouter du code R exécutable

````markdown
```{r}
#| echo: true
# Code R
summary(data)
```
````

## Navigation dans la présentation

- **Flèches** : Naviguer entre les slides
- **Esc** : Vue d'ensemble
- **F** : Plein écran
- **S** : Mode présentateur (avec notes)
- **B** : Tableau noir (si activé)
- **?** : Aide sur les raccourcis

## Modifier le thème

Les couleurs et styles sont définis dans :
- `custom.scss` : Thème principal
- `styles.css` : Styles additionnels

## Ordre des slides

L'ordre des slides dans le fichier `index.qmd` détermine l'ordre de présentation.
Pour réorganiser, déplacez simplement les sections `##` dans le fichier.
