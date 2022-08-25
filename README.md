# react-tuto-19-stock-photo

Application créé en suivant le tutoriel de John Smilga

### mise en pratique basic des apprentissages suivants :

- utilisation de l'api onsplash 
- utilisation d'une variable d'environnement pour l'access key
- infinit scroll (messy !!!)
- search


### mini memo

#### variable d'environnement

- On place en général le fichier `.env` à la racine du projet. Le but étant que le fichier ne soit pas accessible. On n'oublie pas de le mettre dans le `.gitignore`
- les var d'environnement react doivent commencer par `REACT_APP_`
- on n'a pas besoin de guillemet pour donner une  valeur à une var d'environement : `REACT_APP_ACCESS_KEY=macle_secret`
- pour accéder à une var d'environnenemt la syntaxe est `process.env.NOM_VAR`

#### ajouter de nouvelle valeur à un state contenant un tableau 

On destructure renvoie dans le setState un tableau avec les valeurs actuelles du state destructurée et les nouvelles valeurs destructurées

```javascript
setPhoto((oldPhotos) => {
    return [...oldPhotos, ...data];
});
```
