# REST API

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- les verbes HTTP ✔️
- les statuts HTTP ✔️
- les endpoints ✔️
- CORS ✔️
- la nomenclature recommandée pour les routes ✔️

## 💻 J'utilise

### Un exemple personnel commenté ✔️

```javascript
//on l'utilise dans un middlware en haut du fichier,
//il faut bien penser à lui mettre les credentials à true sinon problème de cors lorsqu'on lance le front.
//le 200 est un statut HTTP qui permet de dire que c'est un retour OK qui indique la réussite d'une requête.
app.use(
  cors({
    origin: process.env.FRONTEND_URL ?? "http://localhost:3000",
    optionsSuccessStatus: 200,
    credentials: true,
  })
);
```

### Utilisation dans un projet ✔️

[lien github](https://github.com/WildCodeSchool/2022-03-JS-RemoteFR-Outsiders-P3-SocialTeamConsulting)

Description : Lors du projet STC, nous avons du mettre les cors afin de pouvoir échanger entre le frontend et le backend

### Utilisation en production si applicable ✔️

[lien du projet](https://github.com/WildCodeSchool/2022-03-JS-RemoteFR-Outsiders-P3-SocialTeamConsulting)

Description : 

### Utilisation en environement professionnel ❌ / ✔️

Description :

## 🌐 J'utilise des ressources

### Titre

- https://developer.mozilla.org/fr/docs/Web/HTTP/Status/200#:~:text=Le%20code%20de%20statut%20de,dans%20le%20corps%20du%20message.
- Voici un exemple sur la documentation qui explique ce que signifie le STATUT 200, il est possible de retrouver tout les autres sur le menu à gauche.

## 🚧 Je franchis les obstacles

### Point de blocage ❌ / ✔️

Description:

Plan d'action : (à valider par le formateur)

- action 1 ❌ / ✔️
- action 2 ❌ / ✔️
- ...

Résolution :

## 📽️ J'en fais la démonstration

- J'ai ecrit un [tutoriel](...) ❌ / ✔️
- J'ai fait une [présentation](...) ❌ / ✔️
