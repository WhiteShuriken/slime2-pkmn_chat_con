👾 Overlay Slime Chat - Pokémon Edition

Cet overlay de tchat Twitch est une version hautement personnalisée basée sur le moteur Slime2 (créé par Zaytri). Le code de personnalisation (logique des avatars, commandes tchat et design RPG) a été généré via Gemini.

✨ Présentation

L'overlay transforme votre tchat en une véritable interface de jeu de rôle (RPG) ou de messagerie instantanée (SMS).

Design Épuré : Bulles de texte claires, sans contours agressifs, teintées à la couleur de l'utilisateur.

Grands Avatars : Icônes Pokémon de 120px pour une visibilité maximale.

Mode Conversation : Les messages alternent entre la gauche et la droite de l'écran pour un rendu dynamique.

🚀 Fonctionnement automatique

Attribution Aléatoire : Lors du premier message d'un spectateur, un Pokémon lui est attribué au hasard parmi toutes les générations disponibles.

Persistance : L'utilisateur conserve le même Pokémon durant toute la session de stream.

Logique de Côté : Si un utilisateur enchaîne plusieurs messages, ils restent du même côté. Le côté change dès qu'un nouvel utilisateur prend la parole.

🛠 Commande de personnalisation

Les spectateurs peuvent choisir manuellement leur Pokémon préféré directement depuis le tchat Twitch.

Commande : !pkmn [num_generation] [id_pokemon]

Guide des paramètres :

[num_generation] : Un chiffre de 1 à 8.

1 à 7 : Générations classiques (dossiers gen1 à gen7).

8 : Dossier des formes MEGA (icons_output_genMEGA).

[id_pokemon] : Le numéro du fichier dans le dossier (ex: 25 pour Pikachu).

Exemples d'utilisation :

!pkmn 1 25 : Choisit Pikachu dans la Génération 1.

!pkmn 8 6 : Choisit Dracaufeu Mega dans le dossier MEGA.

Note : La commande est "silencieuse". Lorsqu'un utilisateur l'utilise, le message est automatiquement masqué de l'overlay pour ne pas encombrer visuellement le tchat.

📂 Installation pour OBS

Fichiers : Placez le dossier assets/pokemon_icon/ dans le même dossier que votre fichier overlay-slime-chat.html.

Source Navigateur : Dans OBS, créez une nouvelle source "Navigateur" pointant vers votre fichier local overlay-slime-chat.html.

Permissions : Cochez impérativement la case "Accorder l'accès aux fichiers locaux" pour que les images Pokémon puissent s'afficher.

Code généré avec l'aide de Gemini pour une expérience de stream Pokémon immersive.