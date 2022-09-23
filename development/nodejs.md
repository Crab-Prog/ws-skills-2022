# Titre de la compétence

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- Comment développer en utilisant un système de *livereloading* (`nodemon` par exemple) ✔️
- La connexion de mon application à une base de données avec et sans ORM/ODM (avec `mongodb` puis `mongoose` par exemple) ✔️
- Le développement d'une API REST et GraphQL (avec les packages `express` et `graphql` par exemple) ✔️
- *Bonus : la manipulation des fichiers système avec `fs` et l'utilisation des streams en NodeJS* ❌ / ✔️

## 💻 J'utilise

### Un exemple personnel commenté ❌ / ✔️

```javascript
// this function takes a path to a .md file of the host system and write the HTML version of this file
// the .html file is given back
var express = require('express');
var app = express();
var path = require('path');

const convertMDFileToHTML = (pathToMDfile) => /* ... path to HTML file */

app.get('/', function(req, res) {
    res.sendFile(path.join(__dirname + '/index.html'));
});

app.listen(PORT);
```

### Utilisation dans un projet ❌ / ✔️

[lien github](https://github.com/WildCodeSchool/2022-03-JS-RemoteFR-Outsiders-P3-SocialTeamConsulting)

Description :

### Utilisation en production si applicable❌ / ✔️

[lien du projet](https://social-team-consulting.remote-fr-3.wilders.dev/)

Description :

### Utilisation en environement professionnel ❌ / ✔️

Description :

## 🌐 J'utilise des ressources

### Titre

- lien
- description

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
