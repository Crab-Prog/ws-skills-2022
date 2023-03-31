# Titre de la compétence

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- les différences et points communs entre du code react et du code react native ✔️
- ce que devient et comment est interprêté le code javascript dans une application react native ❌ / ✔️
- les avantages et inconvénients de react native ✔️
- la différence entre react native et expo ❌ / ✔️
- les principales briques qui composent react native (core components) ❌ / ✔️
- comment écrire du style en react native ✔️
- comment est géré le layout en react native ✔️

## 💻 J'utilise

### Un exemple personnel commenté ✔️
En utilisant la librairie Material ui, on importe le component dont on a besoin et on l'utilise. Ici, je rajoute le style directement grâce à la propriété "style".
On remarque qu'on n'écrira pas margin-top mais marginTop. 
```js
import React from 'react'
import { Button } from '@react-native-material/core'

const ButtonComponent = ({
    navigation,
    navigationName,
    title, variant,
    color
}) => {
    return (
        <Button
            style={{ marginTop: 20, marginBottom: 20 }}
            title={title}
            variant={variant}
            color={color}
            onPress={() => {
                navigation.navigate(navigationName)
            }} />
    )
}

export default ButtonComponent
```

### Utilisation dans un projet ✔️

[lien github](https://github.com/WildCodeSchool/2209-wns-hamilton-flashupload-mobile/blob/main/src/pages/Account.js)

Description : Utilisation des components de react native et de material ui. Import de StyleSheet pour ajouter le style css.

### Utilisation en production si applicable❌ / ✔️

[lien du projet](...)

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
