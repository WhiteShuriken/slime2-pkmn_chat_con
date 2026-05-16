👾 Overlay Slime Chat - Pokémon Edition

Cet overlay de tchat Twitch est basé sur le moteur Slime2 (créé par Zaytri). Il a été personnalisé pour afficher les messages sous forme de bulles de conversation (style RPG/SMS) accompagnées d'avatars Pokémon aléatoires.

🚀 Fonctionnement

À chaque premier message d'une session, un Pokémon est attribué aléatoirement à l'utilisateur.

L'utilisateur garde la même icône pendant toute la durée de la session (jusqu'au rechargement de l'overlay).

Les messages alternent entre la gauche et la droite de l'écran pour simuler une conversation.

🛠 Commande de personnalisation

Les spectateurs peuvent choisir manuellement leur Pokémon préféré directement depuis le tchat Twitch.

Commande :
!pkmn [num_generation] [id_pokemon]

Paramètres :

[num_generation] : Un chiffre de 1 à 8.

1 à 7 correspondent aux dossiers icons_output_gen1 à gen7.

8 correspond au dossier icons_output_genMEGA.

[id_pokemon] : Le numéro du fichier dans le dossier (ex: 25 pour Pikachu).

Exemples :

!pkmn 1 25 : Choisit le Pokémon n°025 dans le dossier de la Génération 1.

!pkmn 8 6 : Choisit le Pokémon n°006 dans le dossier MEGA.

Note : Lorsqu'un utilisateur utilise cette commande, le message est automatiquement masqué de l'overlay pour ne pas encombrer le tchat visuel.

📂 Installation locale

Pour utiliser cet overlay dans OBS :

Assure-toi d'avoir le dossier assets/pokemon_icon/ au même niveau que ton fichier HTML.

Ajoute le fichier overlay-slime-chat.html comme Source Navigateur dans OBS.

Coche la case "Accorder l'accès aux fichiers locaux".