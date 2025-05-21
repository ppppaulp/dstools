lien du Cloud run : https://dstools-api-32184514091.europe-west1.run.app/

CHUNG Theodore : theotrou (roles:tout)
BENZAQUEN Kevin : KevBenz (roles:tout)
PITIOT Paul: ppppaulp (roles:tout)

# 🌐 Mini API FastAPI – Projet Cloud (GCP)

Cette mini-API a été développée en Python avec **FastAPI**, et déployée sur **Google Cloud Platform** via **Docker** et **Cloud Run**.

Elle permet :
- de lire et écrire des données dans un fichier CSV sur **Google Cloud Storage (GCS)**,
- de générer une **blague aléatoire** en français avec **Vertex AI** (modèle Gemini).

---

## 🚀 Endpoints de l'API

| Méthode | Endpoint     | Description                                                                 |
|---------|--------------|-----------------------------------------------------------------------------|
| GET     | `/hello`     | Affiche un message de bienvenue                                             |
| GET     | `/status`    | Renvoie la date/heure actuelle du serveur                                   |
| GET     | `/data`      | Lit un fichier CSV depuis GCS et le retourne                               |
| POST    | `/data`      | Ajoute une ligne à ce fichier CSV sur GCS                                   |
| GET     | `/joke`      | Renvoie une blague générée par IA via Vertex AI Gemini                      |

---


## Technologies utilisées

- Python 3.11 + FastAPI
- Docker
- Google Cloud Storage (GCS)
- Vertex AI / Gemini (ou fallback local)
- Google Cloud Run
- GitHub

---

## Lancement en local

### 1. Cloner le projet

```bash
git clone https://github.com/theotrou/dstools-api.git
cd dstools-api
