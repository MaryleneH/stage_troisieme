# ✅ Checklist de Démarrage Rapide

## Pour activer la présentation en ligne

### Étape 1: Fusionner la branche ✓
```bash
# Fusionner cette branche vers main
git checkout main
git merge copilot/create-presentation-structure
git push origin main
```

OU directement sur GitHub:
1. Aller sur la Pull Request
2. Cliquer sur "Merge pull request"
3. Confirmer la fusion

### Étape 2: Configurer GitHub Pages ✓
1. Aller dans les paramètres du dépôt (`Settings`)
2. Cliquer sur `Pages` dans le menu de gauche
3. Sous `Source`, sélectionner `GitHub Actions`
4. Enregistrer (il n'y a peut-être rien à cliquer, c'est automatique)

### Étape 3: Vérifier le déploiement ✓
1. Aller dans l'onglet `Actions`
2. Voir le workflow "Publish Quarto to GitHub Pages" en cours
3. Attendre qu'il se termine (icône verte ✓)
4. La présentation sera disponible à:
   **https://maryleneh.github.io/stage_troisieme/**

## Personnalisation (optionnel)

### Ajouter un logo
- [ ] Créer ou obtenir un logo (format PNG, 200x200px recommandé)
- [ ] Le placer dans `images/logo.png`
- [ ] Dans `_quarto.yml`, décommenter la ligne `logo: images/logo.png`
- [ ] Commiter et pousser les changements

### Ajouter des images à la présentation
- [ ] Placer les images dans le dossier `images/`
- [ ] Dans `index.qmd`, ajouter: `![Description](images/nom-image.png)`
- [ ] Commiter et pousser

### Modifier le contenu
- [ ] Ouvrir `index.qmd`
- [ ] Modifier le texte des slides
- [ ] Ajouter/supprimer des slides si besoin
- [ ] Commiter et pousser

### Changer les couleurs
- [ ] Ouvrir `custom.scss`
- [ ] Modifier les variables de couleur:
  ```scss
  $presentation-heading-color: #votre-couleur;
  $link-color: #votre-couleur;
  ```
- [ ] Commiter et pousser

## Test local (optionnel, pour développeurs)

### Prérequis
- [ ] Installer Quarto: https://quarto.org/docs/get-started/
- [ ] Installer R: https://www.r-project.org/
- [ ] Cloner le dépôt localement

### Commandes
```bash
# Prévisualiser la présentation
quarto preview

# Générer la présentation
quarto render
```

## Résolution de problèmes

### Le workflow échoue
1. Aller dans `Actions`
2. Cliquer sur le workflow qui a échoué
3. Lire les logs d'erreur
4. Corriger le problème
5. Pousser les corrections

### La page ne s'affiche pas
1. Vérifier que GitHub Pages est activé (Settings > Pages)
2. Vérifier que le workflow a réussi (Actions)
3. Attendre quelques minutes
4. Vider le cache du navigateur (Ctrl+Shift+R)
5. Vérifier l'URL: https://maryleneh.github.io/stage_troisieme/

### Les changements ne s'affichent pas
1. Vérifier que les changements sont poussés vers `main`
2. Vérifier que le workflow s'est exécuté
3. Vider le cache du navigateur
4. Attendre 2-3 minutes

## Utilisation de la présentation

### Mode présentation
- Ouvrir l'URL de la présentation
- Appuyer sur `F` pour le plein écran
- Utiliser les flèches pour naviguer

### Mode présentateur
- Appuyer sur `S` pour ouvrir la vue présentateur
- Une nouvelle fenêtre s'ouvre avec:
  - La slide actuelle
  - La slide suivante
  - Les notes du présentateur
  - Un chronomètre

### Raccourcis clavier
- `→` ou `Espace` : Slide suivante
- `←` : Slide précédente
- `Esc` : Vue d'ensemble
- `F` : Plein écran
- `S` : Mode présentateur
- `B` : Tableau noir
- `?` : Aide

## Documentation

Pour plus de détails, consultez:
- `README.md` - Documentation principale
- `GUIDE.md` - Guide complet
- `DEPLOY.md` - Guide de déploiement
- `STRUCTURE.md` - Structure de la présentation
- `EXAMPLES.md` - Exemples de code R
- `SUMMARY.md` - Résumé du projet

## Support

Pour toute question:
1. Consulter la documentation Quarto: https://quarto.org/docs/presentations/
2. Consulter les fichiers de documentation du projet
3. Vérifier les logs dans Actions si problème de déploiement

---

✨ **Bonne présentation!** ✨
