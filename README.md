# 👾 Overlay Slime Chat - Pokémon RPG Edition

![Engine](https://img.shields.io/badge/Engine-Slime2-blueviolet?style=for-the-badge)
![Customization](https://img.shields.io/badge/Custom--Code-Gemini-orange?style=for-the-badge)
![Platform](https://img.shields.io/badge/Platform-Twitch-6441a5?style=for-the-badge&logo=twitch&logoColor=white)

Une version hautement personnalisée de l'overlay de chat **Slime2** (créé par Zaytri), conçue pour transformer l'interaction de votre stream en une interface de jeu de rôle Pokémon immersive.

---

## ✨ Caractéristiques principales

L'overlay a été intégralement repensé pour offrir une expérience visuelle unique et épurée :

* **🎨 Design "SMS / RPG Clean"** : Suppression totale des bordures, contours et effets néon pour un rendu moderne et minimaliste.
* **🫧 Bulles Dynamiques** : Les messages apparaissent dans des bulles claires, teintées à 15% de la couleur Twitch de l'utilisateur sur un fond blanc pur.
* **🖼️ Avatars Pokémon XL** : Icônes agrandies à **120px** pour une visibilité maximale.
* **💬 Logique de Conversation** : 
    * Le pseudo est placé au-dessus de la bulle de message, aligné horizontalement avec l'avatar.
    * Le bloc complet s'aligne automatiquement à gauche ou à droite.
    * Si un utilisateur parle plusieurs fois de suite, ses messages restent du même côté pour simuler une discussion réelle.
* **💾 Persistance de Session** : Attribution automatique d'un Pokémon aléatoire au premier message, conservé durant toute la session de stream.

---

## 🛠️ Commandes pour les spectateurs

Les spectateurs peuvent choisir manuellement leur Pokémon préféré directement depuis le tchat Twitch.

### Sélection manuelle
**Syntaxe :** `!pkmn [num_generation] [id_pokemon]`

| Paramètre | Valeur | Description |
| :--- | :--- | :--- |
| **[num_generation]** | `1` à `7` | Dossiers de générations classiques |
| | `8` | Dossier des formes **MEGA** |
| **[id_pokemon]** | `Nombre` | Le numéro de l'icône dans le dossier (ex: `25` pour Pikachu) |

### Exemples
* `!pkmn 1 25` : Sélectionne Pikachu (Gen 1).
* `!pkmn 8 6` : Sélectionne Méga-Dracaufeu (Dossier Mega).

> [!IMPORTANT]
> La commande est **silencieuse**. Elle est traitée par l'overlay pour mettre à jour l'avatar, mais le message n'est pas affiché à l'écran pour garder le tchat propre.

---

## 📂 Structure des fichiers

Pour un fonctionnement correct sur votre PC, respectez cette hiérarchie :

```text
/votre-dossier-overlay
├── overlay-slime-chat.html    <-- Fichier unique (Code fusionné)
├── assets/
│   └── pokemon_icon/
│       ├── icons_output_gen1/ (pkmn_000.png, pkmn_001.png...)
│       ├── icons_output_gen2/
│       ├── ...
│       └── icons_output_genMEGA/
```

---

## 🚀 Installation dans OBS

1.  Placez le fichier `overlay-slime-chat.html` et le dossier `assets` dans le même répertoire.
2.  Dans **OBS Studio**, ajoutez une source **Navigateur**.
3.  Cochez **"Fichier local"** et sélectionnez `overlay-slime-chat.html`.
4.  **CRUCIAL :** Cochez la case **"Accorder l'accès aux fichiers locaux"** en bas des propriétés de la source pour charger les images Pokémon.
5.  Définissez la taille de la source (ex: 1920x1080) et rafraîchissez le cache si nécessaire.

---

## 📝 Crédits

* **Moteur de base :** [Slime2](https://slime2.stream) par **Zaytri**.
* **Personnalisation & Logique :** Design et code personnalisé générés via **Gemini** pour une expérience de stream unique.

---
*Fait avec ❤️ pour la communauté Pokémon sur Twitch.*