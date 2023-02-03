# GraphQL

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- la différence entre REST et GraphQL ✔️
- les besoins auxquels répond GraphQL ✔️
- la définition d'un schéma ✔️
- Query ✔️
- Mutation ✔️
- Subscription ❌ / ✔️

## 💻 J'utilise

### Un exemple personnel commenté ✔️

```  
const [addUser] = useMutation(graphql.ADD_USER,
    {
      variables: {
        username: userInfos.username,
        email: userInfos.email,
        passwordraw: userInfos.passwordraw,
        type: userInfos.type
      }
    }); 
```
Pour envoyer des informations via graphql, nous devons utiliser une mutation, créée au préalable dans le backend.
Ici, on désire ajouter un utilisateur, on lui envoyer donc les variables qu'il attend.

```
export const ADD_USER = gql`
mutation Mutation($username: String!, $email: String!, $passwordraw: String!, $type: String!) {
  addUser(username: $username, email: $email, passwordraw: $passwordraw, type: $type) {
    username
    email
  }
}
`;
```
Dans un dossier séparé, on déclare notre ADD_USER.
Le point d'exclamation que l'on voit sur les types des variables signifie qu'elle est obligatoire, il faudra donc lui passer les éléments qu'il attend (en obligatoire) afin que la requête puisse fonctionner.

Le **backend** va avoir un dossier pour les schémas : qui permet de typer les éléments attendu.

```
type Mutation {
  addUser(
    username: String!
    email: String!
    passwordraw: String!
    role: String
    type: String!
    period: String
    renew: Boolean
  ): UserType
}
```
On retrouve le point d'exclamation...

Ensuite, nous avons le dossier des resolvers qui permet d'ajoute les Query ou les Mutation.
Pour continuer avec l'ajout d'un utilisateur:
```
  Mutation: {
    addUser: (
      _: any,
      {
        username,
        email,
        passwordraw,
        type,
        period,
        renew,
      }: {
        username: string;
        email: string;
        passwordraw: string;
        type: string;
        period: "monthly" | "yearly";
        renew: boolean;
      },
      context: any,
      infos: any
    ) => {
      const fields = getFieldNames(infos);
      return new UserController().createUser({
        username,
        email,
        passwordraw,
        type,
        period,
        renew,
      });
    },
}
```
Dans le return, on voit qu'on fait appelle à une méthode du controller UserController.
C'est à cet endroit que nous allons pouvoir écrire la logique du code, en ajoutant les messages d'erreur s'il y a un problème, en vérifiant si l'email existe déjà..
S'il n'y a pas de soucis alors :
```
 const user = await this.db.create({
      username,
      email,
      password,
      role: "user",
    });
    await this.db.save(user);
```
On save l'utilisateur dans la base de données.

### Utilisation dans un projet ✔️

[lien github](https://github.com/WildCodeSchool/2209-wns-hamilton-flashupload-front/blob/dev/src/components/Signup.tsx)

Description :

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
