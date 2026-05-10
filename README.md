# TrailMate 🏔️

Coach trail IA personnel — Plans d'entraînement, suivi des séances, Strava sync.

## Déploiement en 5 étapes

### 1. Créer le repo GitHub
1. Va sur [github.com/new](https://github.com/new)
2. Nom du repo : **`trailmate`** (exactement)
3. Visibilité : **Public**
4. Clique "Create repository"

### 2. Uploader les fichiers
```bash
git clone https://github.com/Dblp01/trailmate
cd trailmate
# Copie index.html dans ce dossier
git add .
git commit -m "TrailMate initial"
git push
```
Ou via l'interface GitHub : "uploading an existing file" → glisse `index.html`

### 3. Activer GitHub Pages
1. Settings du repo → Pages
2. Source : "Deploy from a branch"
3. Branch : **main**, dossier : **/ (root)**
4. Save → ton site sera sur `https://dblp01.github.io/trailmate`

### 4. Configurer Strava
Sur [strava.com/settings/api](https://www.strava.com/settings/api) :
- Nom : `TrailMate`
- Site Web : `https://dblp01.github.io`
- **Domaine du rappel : `dblp01.github.io`**

Récupère ton **Client ID** et **Client Secret**.

### 5. Connecter dans l'appli
1. Ouvre `https://dblp01.github.io/trailmate`
2. Entre ta clé API Anthropic
3. Va dans Strava → "Configurer" → entre Client ID + Secret
4. Clique "Se connecter avec Strava" ✅

## Utilisation
- **Plans IA** : crée un plan généré semaine par semaine
- **Séances** : saisie manuelle + sync Strava automatique
- **Coach IA** : conversation avec contexte de tes données réelles
- **Objectifs** : calendrier de tes courses avec compte à rebours
