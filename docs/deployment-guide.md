# Guide de déploiement GitHub Pages

Ce guide est écrit pour quelqu'un qui a **un compte GitHub mais peu ou pas d'expérience** avec MkDocs, Markdown et GitHub Pages.

## Ce que contient déjà ce projet

- le contenu de ton site
- la configuration **MkDocs Material**
- les diagrammes **Mermaid**
- le workflow **GitHub Actions** pour publier automatiquement

## Option la plus simple

Le plus simple est :

1. créer un dépôt GitHub
2. y envoyer ces fichiers
3. activer GitHub Pages via GitHub Actions
4. laisser GitHub construire et publier le site

## Étape 1 — Créer le dépôt GitHub

Dans GitHub :

1. clique sur **New repository**
2. nom du dépôt : `rodrigo-architecture-portfolio`
3. laisse le dépôt en **Public**
4. clique sur **Create repository**

## Étape 2 — Envoyer les fichiers

### Méthode la plus facile

1. télécharge le dossier ou le fichier ZIP
2. dans ton nouveau dépôt GitHub, clique sur **uploading an existing file**
3. glisse tous les fichiers du projet
4. fais le commit sur `main`

## Étape 3 — Remplacer ton nom d'utilisateur GitHub

Ouvre le fichier `mkdocs.yml` dans GitHub et remplace :

- `YOUR_GITHUB_USERNAME`

par ton vrai identifiant GitHub.

## Étape 4 — Activer GitHub Pages

Dans le dépôt :

1. va dans **Settings**
2. clique sur **Pages**
3. dans **Build and deployment**
4. choisis **Source = GitHub Actions**

Tu n'as rien d'autre à configurer.

## Étape 5 — Laisser GitHub publier

Après ton premier push, va dans l'onglet **Actions**. Tu verras le workflow :

- **Deploy MkDocs to GitHub Pages**

Quand il sera terminé avec succès, ton site sera disponible à une adresse semblable à :

`https://ton-username.github.io/rodrigo-architecture-portfolio/`

## Modifier le contenu plus tard

Tu peux modifier le site directement dans GitHub :

1. ouvre un fichier `.md`
2. clique sur l'icône crayon
3. modifie le texte
4. commit

Le site sera redéployé automatiquement.

## Tester localement plus tard (optionnel)

Tu pourras faire ça quand tu seras prêt.

### Installer Python

Installe Python sur ton ordinateur.

### Installer les dépendances

```bash
pip install -r requirements.txt
```

### Lancer le site localement

```bash
mkdocs serve
```

Puis ouvre :

`http://127.0.0.1:8000`

## Ordre conseillé pour toi

Je te recommande cet ordre :

1. publier le site tel quel
2. vérifier que GitHub Pages fonctionne
3. personnaliser les textes et liens
4. ajouter ensuite ton domaine personnalisé, si tu veux
