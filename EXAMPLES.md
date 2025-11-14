# Exemples de code R pour la présentation

## Introduction

Ce fichier contient des exemples de code R que vous pouvez intégrer dans votre présentation Quarto si nécessaire.

## Exemple 1 : Graphique simple

```r
# Créer un graphique simple
library(ggplot2)

data <- data.frame(
  categorie = c("Prompt faible", "Prompt moyen", "Prompt fort"),
  qualite = c(30, 60, 95)
)

ggplot(data, aes(x = categorie, y = qualite, fill = categorie)) +
  geom_bar(stat = "identity") +
  labs(title = "Qualité de la réponse selon le prompt",
       y = "Qualité (%)",
       x = "Type de prompt") +
  theme_minimal()
```

## Exemple 2 : Tableau de données

```r
# Créer un tableau comparatif
library(knitr)

comparaison <- data.frame(
  Critère = c("Clarté", "Précision", "Contexte", "Structure"),
  "Prompt faible" = c("❌", "❌", "❌", "❌"),
  "Prompt fort" = c("✅", "✅", "✅", "✅"),
  check.names = FALSE
)

kable(comparaison, caption = "Comparaison des prompts")
```

## Intégration dans index.qmd

Pour inclure du code R dans votre présentation, utilisez des chunks R :

````markdown
## Titre de la slide

```{r}
#| echo: true
#| eval: true
#| fig-width: 8
#| fig-height: 4

# Votre code R ici
```
````

## Conseils

- Utilisez `echo: true` pour afficher le code
- Utilisez `eval: true` pour exécuter le code
- Utilisez `echo: false` pour cacher le code mais afficher les résultats
- Ajustez `fig-width` et `fig-height` pour les graphiques

## Installation des packages nécessaires

Si vous ajoutez du code R, assurez-vous d'installer les packages :

```r
install.packages(c("ggplot2", "knitr", "dplyr", "tidyr"))
```

Et mettez à jour le workflow GitHub Actions dans `.github/workflows/publish.yml` :

```yaml
- name: Install R dependencies
  run: |
    install.packages(c("rmarkdown", "knitr", "ggplot2", "dplyr", "tidyr"))
  shell: Rscript {0}
```
