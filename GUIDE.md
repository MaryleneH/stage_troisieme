# 📚 Guide Complet - Présentation Prompt Engineering

## 🎯 Objectif

Cette présentation vise à introduire le Prompt Engineering à un public de collégiens (3ème) de manière accessible et interactive.

## 📁 Fichiers du projet

### Fichiers principaux
- **`index.qmd`** - Contenu de la présentation (10+ slides)
- **`_quarto.yml`** - Configuration Quarto pour le rendu
- **`README.md`** - Documentation principale du projet

### Fichiers de style
- **`custom.scss`** - Thème personnalisé (SCSS)
- **`styles.css`** - Styles CSS additionnels

### Fichiers de configuration
- **`.gitignore`** - Fichiers à exclure du dépôt
- **`.nojekyll`** - Active GitHub Pages pour Quarto
- **`.github/workflows/publish.yml`** - Workflow de déploiement automatique

### Documentation
- **`DEPLOY.md`** - Guide de déploiement GitHub Pages
- **`EXAMPLES.md`** - Exemples de code R
- **`STRUCTURE.md`** - Structure détaillée de la présentation

### Ressources
- **`images/`** - Dossier pour images et logo

## 🚀 Démarrage rapide

### Option 1 : Modification directe sur GitHub
1. Éditez `index.qmd` directement sur GitHub
2. Commitez les modifications sur la branche `main`
3. Le déploiement se fait automatiquement via GitHub Actions

### Option 2 : Développement local
1. Installez [Quarto](https://quarto.org/docs/get-started/)
2. Installez [R](https://www.r-project.org/)
3. Clonez le dépôt
4. Exécutez `quarto preview` pour prévisualiser
5. Exécutez `quarto render` pour générer

## 📝 Contenu de la présentation

1. **Introduction** - Bienvenue et présentation du sujet
2. **Définition** - Qu'est-ce qu'un prompt ?
3. **Importance** - Pourquoi apprendre le Prompt Engineering ?
4. **Principes** - Les 3 principes de base
5. **Exemples** - Comparaisons avant/après
6. **Techniques** - 4 techniques avancées
7. **Exercice** - Pratique interactive
8. **Erreurs** - Ce qu'il faut éviter
9. **Ressources** - Outils et liens utiles
10. **Conclusion** - Récapitulatif et questions

## 🎨 Personnalisation

### Modifier le contenu
Éditez `index.qmd` en suivant la syntaxe Markdown/Quarto.

### Modifier les couleurs
Éditez `custom.scss` pour changer les couleurs du thème :
```scss
$presentation-heading-color: #2c3e50;  // Couleur des titres
$link-color: #3498db;                   // Couleur des liens
```

### Ajouter des images
1. Placez l'image dans le dossier `images/`
2. Référencez-la dans `index.qmd` :
```markdown
![Description](images/mon-image.png)
```

### Ajouter un logo
1. Créez un fichier `images/logo.png` (200x200px recommandé)
2. Décommentez la ligne `logo:` dans `_quarto.yml`

## 🔧 Configuration GitHub Pages

### Première fois
1. Allez dans **Settings** > **Pages**
2. Source : **GitHub Actions**
3. Enregistrez

### Vérifier le déploiement
- Onglet **Actions** : voir les workflows
- URL : `https://maryleneh.github.io/stage_troisieme/`

## 🎓 Fonctionnalités de la présentation

### Éléments interactifs
- **Slides progressives** : Le contenu apparaît au clic
- **Tableaux à onglets** : Exemples organisés en panneaux
- **Notes du présentateur** : Appuyez sur `S` pendant la présentation
- **Tableau noir** : Dessinez sur les slides (icône en bas)

### Navigation
- **Flèches** : Avancer/reculer
- **Esc** : Vue d'ensemble de toutes les slides
- **F** : Plein écran
- **?** : Aide sur les raccourcis

## 📊 Ajout de code R (optionnel)

Si vous voulez ajouter des visualisations avec R :

1. Consultez `EXAMPLES.md` pour des exemples
2. Ajoutez des chunks R dans `index.qmd`
3. Mettez à jour les dépendances dans le workflow

## 🛠️ Dépannage

### La présentation ne se génère pas
- Vérifiez la syntaxe YAML dans `index.qmd` (---...---)
- Assurez-vous que tous les fichiers référencés existent
- Consultez les logs dans l'onglet Actions

### Le déploiement échoue
- Vérifiez les permissions dans Settings > Actions
- Assurez-vous que GitHub Pages est activé
- Consultez les logs du workflow

### Les styles ne s'appliquent pas
- Videz le cache du navigateur
- Attendez quelques minutes après le déploiement
- Vérifiez que `custom.scss` et `styles.css` sont bien référencés

## 📚 Ressources

- [Documentation Quarto](https://quarto.org/docs/presentations/revealjs/)
- [Syntaxe Markdown](https://www.markdownguide.org/)
- [Reveal.js (moteur de présentation)](https://revealjs.com/)
- [GitHub Pages](https://pages.github.com/)

## 🔄 Workflow de mise à jour

1. **Éditer** le contenu dans `index.qmd`
2. **Commiter** les modifications
3. **Pousser** vers la branche `main`
4. **Attendre** le déploiement automatique (2-3 minutes)
5. **Vérifier** la présentation en ligne

## ✅ Checklist de lancement

- [x] Structure du projet créée
- [x] Fichier de présentation (`index.qmd`)
- [x] Configuration Quarto (`_quarto.yml`)
- [x] Styles personnalisés
- [x] Workflow GitHub Actions
- [x] Documentation complète
- [ ] Ajouter un vrai logo (remplacer `images/logo.html`)
- [ ] Personnaliser les couleurs selon les préférences
- [ ] Ajouter des images spécifiques au contenu
- [ ] Tester le déploiement sur la branche main
- [ ] Partager l'URL finale

## 🎯 Prochaines étapes recommandées

1. **Fusionner** cette branche vers `main` pour activer le déploiement
2. **Personnaliser** le contenu selon les besoins spécifiques
3. **Ajouter** des images et exemples visuels
4. **Tester** la présentation en mode présentateur
5. **Partager** l'URL avec Naela

## 📞 Support

Pour toute question sur Quarto : [quarto.org/docs/presentations](https://quarto.org/docs/presentations/)

---

**Bon courage avec la présentation ! 🚀**
