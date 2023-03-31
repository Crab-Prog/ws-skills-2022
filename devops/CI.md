# Integration continue

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- les enjeux de l'integration continue ✔️
- la mise en place d'une github action ✔️

## 💻 J'utilise

### Un exemple personnel commenté ✔️

Sur le Front de notre site web, nous avons un fichier yaml qui va déclencher la commande pour vérifier si les tests passent, pour améliorer notre intégration continue.
Ici, le test se lance lorsqu'on effectuera une PR d'une branche vers une autre branche, si le test échoue alors il ne sera pas possible de merger.
```yml
name: Tests

on:
  push:
  workflow_dispatch:

jobs:
  test-front:
    runs-on: ubuntu-latest
    steps:
      - name: Check out code
        uses: actions/checkout@v3
      - name: Goto src and run tests
        run: npm i && npm test
```


### Utilisation dans un projet ✔️

[lien github](https://github.com/WildCodeSchool/2209-wns-hamilton-flashupload-back/blob/staging/.github/workflows/docker_push_staging.yml)

Description : Lien vers le fichier yqml qui contient le code pour compiler et push sur la pre-prod

### Utilisation en production si applicable ✔️

[lien du projet](https://github.com/WildCodeSchool/2209-wns-hamilton-flashupload-back/blob/staging/.github/workflows/docker_push_staging.yml)

Description : Idem

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
