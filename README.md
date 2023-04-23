# Agence_location_voiture

## Stack technique
Je souhaite utiliser SASS (préprocesseur CSS), j'ai besoin de NPM (gestionnaire de package), je télécharge et installe node JS sur la machine.

- Node JS
- NPM (livré avec node JS) 
    - Exemple de mise à jour : `npm install -g npm@9.6.5`
- SASS


## NPM

Version : `npm -v`

Initialiser un projet : `npm init -y` 
- `y` : si on veux pas repondre au question (nom, version ... de l'app)
- Création d'un fichier `package.json`

Installer une dépendance: `nmp install -g <nom_de_la_dependance>`
- `g` : global (puex être lancé à partir de n'importe quel emplacement) sinon ne rien mettre et dispos seulement dans le projet.

Installer NODE SASS : `npm install node-sass`
- Npm génère le dossier `node_modules` et installe la dépendance.

Ajoute un script dans `package.json`
````
"sass:compil": "node-sass assets/css/sass/main.scss assets/css/style.css",
"sass:watch": "node-sass assets/sass/main.scss assets/css/style.css -w"
````

Puis on lance la compilation du `scss` en `css` : `npm run sass:watch`

