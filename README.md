# coding-project-template



Tâche 5 : Déployer avec GitHub Pages

    Pour déployer votre application react sur GitHub, vous devez installer gh-pages. Cela vous permet de l’utiliser comme un outil pour déployer votre projet sur GitHub Pages. Exécutez la commande donnée dans le terminal

        1
        npm install gh-pages --save-dev

Ajoutez les lignes données avant "build": "vite build" dans le fichier package.json.

    1
    2

    "predeploy": "npm run build",
    "deploy": "gh-pages -d dist",

    Ensuite, dans le fichier vite.config.js, ajoutez cette ligne avant plugins : [react()]

        1
        base: "/VOTRE_NOM_DE_DEPOT",

Remarque : Au lieu de <VOTRE_NOM_DE_DEPOT>, écrivez votre propre nom de dépôt, par exemple, si le nom de votre dépôt GitHub est learning_react, cela devrait ressembler à base: "/learning_react".

Maintenant, exécutez la commande de déploiement dans le terminal pour exécuter le script “deploy” défini dans le fichier package.json, déployant le projet sur GitHub Pages à l’aide de l’outil gh-pages.

    1

    npm run deploy

Remarque : Chaque fois que vous apportez des modifications à votre code, vous devez enregistrer tous vos fichiers et exécuter des commandes git pour ceux-ci.

    Exécutez les commandes git add et git commit pour mettre à jour les modifications dans votre code. Ensuite, exécutez la commande git push pour mettre à jour votre dépôt GitHub pour une gestion correcte du code.

    Allez sur votre dépôt GitHub. Ensuite, naviguez vers le dépôt de votre site que vous avez créé.

    Sous le nom de votre dépôt, cliquez sur Paramètres.

    Naviguez dans la barre de navigation à gauche. Dans la section Code et automatisation de la barre latérale, cliquez sur Pages.

    Onglet Paramètres avec Pages entouré

    Vous verrez la page montrée ci-dessous. Cliquez sur le menu déroulant où vous voyez Aucun, puis cliquez sur gh-pages, puis cliquez sur le bouton Enregistrer.

    Rafraîchissez votre page à nouveau, et vous verrez le lien, comme ci-dessous. Au lieu de shoppingreact, vous verrez le nom de votre dépôt GitHub.

    Remarque : Si vous ne parvenez pas à voir le lien, veuillez attendre (1-2) minutes et rafraîchir la page à nouveau.

    Cliquez sur le lien généré ci-dessus pour voir votre site web en direct.

    Remarque :
    1. Si vous n’avez apporté aucune modification à votre application React par défaut, vous devriez voir une sortie similaire pour la tâche 3, étape 6, comme montré ci-dessous.
    2. Après le déploiement sur GitHub Pages, il peut falloir un certain temps pour que tous les contenus et images apparaissent correctement. Veuillez attendre quelques minutes supplémentaires pour que l’application se charge complètement.

En respectant ces directives, vous pouvez maintenir un dépôt GitHub bien organisé et efficace, garantissant que votre travail est stocké en toute sécurité et facilement accessible à vous et vos collaborateurs.
Author(s)

Richa Arora
© IBM Corporation. Tous droits réservés.
