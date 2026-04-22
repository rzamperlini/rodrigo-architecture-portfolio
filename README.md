# Rodrigo Zamperlini - Architecture Portfolio

Portfolio professionnel construit avec **MkDocs Material**, **Markdown** et **Mermaid**, prêt pour **GitHub Pages**.

## Démarrage local

```bash
pip install -r requirements.txt
mkdocs serve
```

Puis ouvrir `http://127.0.0.1:8000`.

## Build local

```bash
mkdocs build
```

## Déploiement GitHub Pages

Le dépôt inclut déjà un workflow GitHub Actions.

1. Crée un dépôt GitHub nommé `rodrigo-architecture-portfolio`
2. Envoie les fichiers sur la branche `main`
3. Dans GitHub : **Settings > Pages > Build and deployment > Source = GitHub Actions**
4. Le site sera publié automatiquement après le push

## Personnalisation importante

Avant de publier, remplace `YOUR_GITHUB_USERNAME` dans `mkdocs.yml` par ton vrai nom d'utilisateur GitHub.
