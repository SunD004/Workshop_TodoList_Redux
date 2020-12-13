# React Native préparation de l'environement

#### Doc officiel
* https://reactnative.dev/docs/environment-setup

#### Node.JS
* https://github.com/nodesource/distributions/blob/master/README.md

#### Installer JAVA 
* #### Ubuntu
    * sudo add-apt-repository ppa:webupd8team/java
    * sudo apt-get update
    * sudo apt-get install oracle-java8-installer
    * sudo apt-get install oracle-java8-set-default
* #### Fedora
    * sudo dnf install java-11-openjdk.x86_64

**Android studio** (Si vous voulez utiliser un émulateur android. Si vous avez un téléphone android ce n'est pas nécéssaire)
* **https://developer.android.com/studio/index.html (installation via le dossier)**
* **ou via ubuntu software pour ubuntu**
* **ou via les paquets (ubuntu/fedora)**
* https://fedoraproject.org/wiki/Android_Studio

## Installer les dependances de android-studio
#### Ubuntu
    sudo apt-get install libc6:i386 libncurses5:i386 libstdc++6:i386 lib32z1 libbz2-1.0:i386
#### Fedora
    sudo yum install zlib.i686 ncurses-libs.i686 bzip2-libs.i686


## Exercice 1 

# Cree son projet react avec expo
    npm install -g expo-cli
    expo init nomduprojet
    Ensuite choissier "blank, a minimal app as clean as an empty canvas" (le 1er) puis cliquer sur entrer

## Exercice 2

### 1er étape

## Une fois que votre projet générer et que vous avez eu 0 erreur nous allons pouvoir lancer l'app sur un téléphone !

    Vous avez 2 choix sois vous télécharger un émulateur de téléphone directement via android studio (nécessite une bonne connexion pour faire le download) sous vous brancher votre téléphone avec votre cable USB a votre PC.

* **Pour télécharger un émulateur sur android-studio rendez-vous dans "Tools -> AVD Manager -> + Create Virtual Device" ensuite selectionner le téléphone que vous voulez (Pixel 2 pour moi) puis cliquez sur Next. Maintenant il faut download l'OS android de votre téléphone, pour notre projet il nous faut un OS API LEVEL 28 il s'appelle 'Pie' ensuite cliquer sur Next cela va lancer un download, à la fin de se download vous cliquez sur Next puis sur Finish**

* **Pour brancher votre téléphone il suffit de brancher votre cable usb de votre ordinateur a votre téléphone. Ensuite vous devez activer le mode développeur sur votre téléphone pour l'activer il suffit de vous rendre dans les paramètres de votre téléphone de cliquer sur 'A propos du téléphone' puis de spam clique votre Numéros de Build, si le mode dev est activé un petit message va apparaître. Si cette méthode fonctionne pas pour vous je vous invite à regarder sur internet en fonction de votre modèle. Puis d'activer le débogage pour que votre téléphone sois reconnu par adb**

* **Si tous est ok vous pouvez faire expo start a la racine du projet ça va vous ouvrir une page web en localhost une fois sur cette page et que vous etes bien brancher avec votre téléphone ou que votre émulateur est bien lancer cliquer sur Run on android device/emulator**

## Exercice 3

#### C'est parti votre environnement travail est pret et vous allez pouvoir coder!


**Votre premier exercice sera de faire une simple TodoList.
Je vous interdis de faire des class component en 2020 !
Si vous ne connaissez pas du tout les functional components je vous invites a regarder comment fonctionne les Hooks pour vous permettre de créer et modifier des states dans un functional component.
Doc officiel sur les Hooks -> https://fr.reactjs.org/docs/hooks-intro.html**

## Exercice 4

#### Bon c'est bien joli mais maintenant on va découvrir REDUX ! :O

* **npm install --save react-redux**
* **npm install redux**
* **Petit gif qui montre le fonctionnement de redux -> https://redux.js.org/assets/images/ReduxDataFlowDiagram-49fa8c3968371d9ef6f2a1486bd40a26.gif**

**Voici quelques liens pour vous aidez à implementer Redux en utilisant la dernière façon de faire (Redux Hooks):**
* -> https://www.youtube.com/watch?v=3zoIigieur0 
* -> https://react-redux.js.org/api/hooks

#### Implementer redux dans son app nécéssite :
* **un reducer (store) qui contient les states de notre app**
* **des actions pour intéragir avec notre store, une action reçois une valeur en parametre et l'envoie en payload au store**
* **des constants pour définir le type de nos actions pour qu'une action modifie tel ou tel state de notre reducer**


**Vous allez maintenant faire le meme exercice mais cette fois en utilisant le framework redux dans votre app**
