# Acceder au dépot Github en SSH

Lancer le terminal dans le dossier `<Home>/.ssh`

Création de la clé privée et publique : `ssh-keygen -o`

Taper un nom pour la clé ex: github

Ne pas entrer de mot de passe sinon il faudra le renseigner à chaque fois.

Une fois les 2 fichiers générés, ouvrir le fichier avec un éditeur CLI (cat, nano vim ...) et copier la clé publique  : `cat ~/.ssh/id_rsa.pub`

Ce rendre sur github dans `settings/SSH/` new ssh key



# Agence de location voiture
 
 [![](https://github.com/Eric-dev13/Agence_location_voiture/blob/main/assets/images/background.jpg)]( https://eric-dev13.github.io/Agence_location_voiture/)

## Stack technique
Je souhaite utiliser SASS (préprocesseur CSS), j'ai besoin de NPM (gestionnaire de package), je télécharge et installe node JS sur la machine.

- Node JS
- NPM (livré avec node JS) 
    - Exemple de mise à jour : `npm install -g npm@9.6.5`
- SASS


## NPM

Version de npm : `npm -v`

Initialiser un projet : `npm init <option>` 

Options :
- `y` : si on veux pas repondre au question (nom, version ... de l'app)
- Création d'un fichier `package.json`

Installer une dépendance: `nmp install <options> <nom_de_la_dependance>`

Options :
- `-g` : Installation global (peux être lancé dans un terminal à partir de n'importe quel emplacement) sinon ne rien mettre et dispos seulement dans le projet.
- `-D` : Développement - Installe la dépendance seulement pour ce projet

INSTALLATION DE SASS

NODE-SASS EST DEPRECIE DEPUIS LA VERSION 5 DE BOOTSTARP

`npm install -D sass`
````
Ajoute un script dans `package.json`
"sass:watch": "sass assets/sass/main.scss assets/css/style.css -w"
````

Puis on lance la compilation du `scss` en `css` : `npm run sass:watch`

Installation d'hugo un générateur de site statique léger
`npm install hugo-bin --save-dev`

````
npm run-script

{
  "scripts": {
    "build": "hugo",
    "create": "hugo new",
    "serve": "hugo server"
  }
}
````

PREFIXER ()
npm install postcss postcss-cli autoprefixer
npx postcss *.css --use autoprefixer -d build/

