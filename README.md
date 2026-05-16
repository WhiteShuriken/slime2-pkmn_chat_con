👾 Overlay Slime Chat - Pokémon RPG Edition

Une version hautement personnalisée de l'overlay de chat Slime2 (créé par Zaytri), conçue pour transformer l'interaction de votre stream en une interface de jeu de rôle Pokémon.

✨ Caractéristiques principales

L'overlay a été intégralement repensé pour offrir une expérience immersive :

🎨 Design "SMS / RPG Clean" : Suppression totale des bordures et contours pour un rendu moderne et épuré.

🫧 Bulles Dynamiques : Les messages apparaissent dans des bulles claires, subtilement teintées selon la couleur de l'utilisateur sur Twitch.

🖼️ Avatars Pokémon XL : Icônes de 100px à 120px pour une visibilité parfaite en plein stream.

💬 Logique de Conversation : Alternance automatique des messages entre la gauche et la droite de l'écran. Si un utilisateur parle plusieurs fois de suite, il reste du même côté.

💾 Persistance de Session : Chaque spectateur se voit attribuer un Pokémon aléatoire dès son premier message et le conserve jusqu'au rechargement de l'overlay.

🛠️ Commandes pour les spectateurs

Les spectateurs peuvent outrepasser l'attribution aléatoire et choisir manuellement leur Pokémon préféré.

Sélection manuelle

Syntaxe : !pkmn [num_generation] [id_pokemon]

Paramètre

Valeur

Description

[num_generation]

1 à 7

Dossiers de générations classiques



8

Dossier des formes MEGA

[id_pokemon]

Nombre

Le numéro de l'icône dans le dossier (ex: 25 pour Pikachu)

Exemples

!pkmn 1 25 : Sélectionne Pikachu (Gen 1).

!pkmn 8 6 : Sélectionne Méga-Dracaufeu (Dossier Mega).

Note : Cette commande est "silencieuse". Elle est traitée par le moteur mais n'est pas affichée dans la bulle de chat pour préserver la propreté de l'overlay.

📂 Structure des fichiers

Pour que l'overlay fonctionne, vos fichiers doivent être organisés ainsi :

/votre-dossier-overlay
├── overlay-slime-chat.html    <-- Fichier principal (Code fusionné)
├── assets/
│   └── pokemon_icon/
│       ├── icons_output_gen1/ (pkmn_000.png, pkmn_001.png...)
│       ├── icons_output_gen2/
│       ├── ...
│       └── icons_output_genMEGA/


🚀 Installation dans OBS

Placez le fichier overlay-slime-chat.html et le dossier assets dans un dossier dédié sur votre PC.

Ouvrez OBS Studio.

Ajoutez une nouvelle source Navigateur.

Cochez "Fichier local" et sélectionnez votre fichier HTML.

IMPORTANT : Cochez la case "Accorder l'accès aux fichiers locaux" (tout en bas des propriétés de la source). Sans cela, les icônes Pokémon ne pourront pas s'afficher.

Réglez la taille de la source sur les dimensions de votre stream (ex: 1920x1080).

📝 Crédits

Moteur de base : Slime2 par Zaytri.

Personnalisation & Logique : Code généré et optimisé via Gemini pour une expérience Pokémon unique.

Fait avec ❤️ pour la communauté Pokémon sur Twitch.