# YC6 - Évaluation affective d'images 

Expérience comportementale interactive utilisant jsPsych.

## 🌐 Accès en ligne (participants)

**URL de l'expérience :** https://lokas21.github.io/zoom/

Ouvrez le lien ci-dessus dans un navigateur récent (Chrome ou Firefox recommandé) pour démarrer l'expérience. Aucune installation n'est requise.

## Structure du dépôt
- `index.html` - Application principale (expérience jsPsych)
- `images/` - Images émotionnelles (sadness, hope)
- `dat_images/` - Dessins DAT (dat1–dat4)
- `config/` - Fichiers de configuration Excel
- `data/` - Dossier de stockage des données participants (CSV téléchargés localement)

## Collecte des données

Les données sont sauvegardées **localement** dans le navigateur du participant. À la fin de l'expérience, un fichier CSV nommé `YC6_data_<horodatage>.csv` est automatiquement téléchargé sur l'ordinateur du participant.

Pour récupérer les données :
1. Demandez aux participants d'envoyer leur fichier CSV par e-mail ou via un lien de partage (ex. OneDrive, Dropbox).
2. Placez les fichiers reçus dans le dossier `data/` de ce dépôt (non suivi par Git, à conserver localement).

## Lancer localement (développement)

```bash
python -m http.server 8000
```
Puis ouvrir : http://localhost:8000/index.html

## Déploiement GitHub Pages

Le déploiement est automatique via GitHub Actions à chaque `push` sur la branche `main`. Voir `.github/workflows/deploy.yml`.

## Contact technique

Pour tout problème technique lié à l'accès ou au fonctionnement de l'expérience, contactez le responsable du dépôt GitHub.
