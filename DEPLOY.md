# Guide de déploiement GitHub Pages

## Configuration initiale de GitHub Pages

1. **Aller dans les paramètres du dépôt**
   - Ouvrez votre dépôt sur GitHub
   - Cliquez sur "Settings" (Paramètres)

2. **Configurer GitHub Pages**
   - Dans le menu de gauche, cliquez sur "Pages"
   - Sous "Source", sélectionnez "GitHub Actions"
   - Enregistrez les modifications

3. **Vérifier les permissions**
   - Dans Settings > Actions > General
   - Sous "Workflow permissions"
   - Assurez-vous que "Read and write permissions" est activé
   - Cochez "Allow GitHub Actions to create and approve pull requests"

## Déploiement automatique

Une fois la configuration terminée :

1. Chaque commit sur la branche `main` déclenche automatiquement :
   - L'installation de Quarto et R
   - La génération de la présentation
   - Le déploiement sur GitHub Pages

2. Vous pouvez suivre le progrès dans l'onglet "Actions" du dépôt

3. La présentation sera disponible à l'adresse :
   `https://maryleneh.github.io/stage_troisieme/`

## Déploiement manuel

Si vous voulez déclencher un déploiement manuellement :

1. Allez dans l'onglet "Actions"
2. Sélectionnez le workflow "Publish Quarto to GitHub Pages"
3. Cliquez sur "Run workflow"
4. Sélectionnez la branche `main`
5. Cliquez sur "Run workflow"

## Dépannage

### Le workflow échoue

- Vérifiez les logs dans l'onglet "Actions"
- Assurez-vous que tous les fichiers nécessaires sont présents
- Vérifiez que le fichier `_quarto.yml` est correctement formaté

### La page ne s'affiche pas

- Attendez quelques minutes après le déploiement
- Videz le cache de votre navigateur
- Vérifiez que GitHub Pages est activé dans les paramètres

### Erreurs de rendu

- Vérifiez la syntaxe dans `index.qmd`
- Assurez-vous que tous les fichiers référencés existent
- Consultez les logs du workflow pour plus de détails

## Mise à jour de la présentation

Pour mettre à jour la présentation :

1. Modifiez `index.qmd` localement ou directement sur GitHub
2. Commitez et poussez les modifications vers `main`
3. Le workflow se déclenche automatiquement
4. La présentation est mise à jour en quelques minutes

## Personnalisation avancée

### Changer le thème

Modifiez `custom.scss` pour personnaliser les couleurs et les styles.

### Ajouter des plugins Reveal.js

Ajoutez des plugins dans la section `revealjs` de `_quarto.yml` :

```yaml
format:
  revealjs:
    plugins:
      - RevealNotes
      - RevealSearch
```

### Utiliser un domaine personnalisé

1. Créez un fichier `CNAME` à la racine avec votre domaine
2. Configurez votre DNS pour pointer vers GitHub Pages
3. Activez le domaine personnalisé dans Settings > Pages
