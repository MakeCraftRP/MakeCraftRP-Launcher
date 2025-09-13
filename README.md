# 🎮 MakeCraftRP Launcher

<div align="center">

![MakeCraftRP Logo](../src/assets/images/icon.png)

**Launcher officiel du serveur Minecraft MakeCraftRP**

[![Version](https://img.shields.io/badge/version-2.2.8-blue.svg)](https://github.com/MakeCraftRP/MakeCraftRP-Launcher)
[![License](https://img.shields.io/badge/license-CC0-green.svg)](LICENSE.md)
[![Electron](https://img.shields.io/badge/Electron-37.2.0-47848F.svg)](https://electronjs.org/)
[![Discord](https://img.shields.io/discord/YOUR_DISCORD_ID?color=7289DA&label=Discord&logo=discord)](https://discord.gg/HMEMeeMkr8)

[📥 Télécharger](#installation) • [📖 Documentation](#utilisation) • [🐛 Signaler un bug](https://github.com/MakeCraftRP/MakeCraftRP-Launcher/issues) • [💬 Discord](https://discord.gg/HMEMeeMkr8)

</div>

## ✨ Fonctionnalités

- 🚀 **Lancement automatique** - Connexion directe au serveur MakeCraftRP
- 👤 **Gestion des comptes** - Support Microsoft et authentification sécurisée
- 🎯 **Gestion intelligente de la RAM** - Allocation automatique optimisée
- 📦 **Gestionnaire de mods** - Installation et mise à jour automatique des mods
- 🎨 **Personnalisation des skins** - Upload et prévisualisation 3D
- 📰 **Actualités intégrées** - News et mises à jour du serveur
- 🔗 **Réseaux sociaux** - Liens directs vers Discord, Instagram, TikTok
- 🌐 **Interface moderne** - Design glassmorphism responsive
- 🔄 **Mises à jour automatiques** - Launcher toujours à jour

## 🖥️ Captures d'écran

<details>
<summary>Voir les captures d'écran</summary>

### Page d'accueil
![Accueil](screenshots/home.png)

### Paramètres
![Paramètres](screenshots/settings.png)

### Gestion des mods
![Mods](screenshots/mods.png)

</details>

## 📋 Prérequis

- **OS:** Windows 10+ / macOS 10.15+ / Linux (Ubuntu 18.04+)
- **RAM:** 4 GB minimum (8 GB recommandé)
- **Java:** 8+ (détection automatique)
- **Connexion Internet** pour les mises à jour et l'authentification

## 📥 Installation

### Téléchargement direct
1. Rendez-vous sur la [page des releases](https://github.com/MakeCraftRP/MakeCraftRP-Launcher/releases)
2. Téléchargez la version correspondant à votre OS :
   - **Windows:** `MakeCraftRP-Launcher-Setup-2.2.8.exe`
   - **macOS:** `MakeCraftRP-Launcher-2.2.8.dmg`
   - **Linux:** `MakeCraftRP-Launcher-2.2.8.AppImage`
3. Lancez l'installateur et suivez les instructions

### Installation depuis les sources
```bash
# Cloner le repository
git clone https://github.com/MakeCraftRP/MakeCraftRP-Launcher.git
cd MakeCraftRP-Launcher

# Installer les dépendances
npm install

# Lancer en mode développement
npm start

# Compiler pour votre plateforme
npm run build
```

## 🚀 Utilisation

### Premier lancement
1. **Authentification** - Connectez-vous avec votre compte Microsoft
2. **Configuration** - Le launcher détecte automatiquement votre configuration Java
3. **Allocation RAM** - Ajustez la mémoire selon vos besoins (recommandé : 4-6 GB)
4. **Mods** - Les mods requis sont téléchargés automatiquement
5. **Jouer** - Cliquez sur "Jouer" pour rejoindre MakeCraftRP !

### Fonctionnalités avancées

#### Gestion des comptes
- Support de plusieurs comptes Microsoft
- Basculement rapide entre comptes
- Authentification sécurisée avec tokens

#### Personnalisation
- **Skins personnalisés** - Format PNG 64x64 max
- **Paramètres de lancement** - Options avancées Java
- **Thème responsive** - Interface adaptative

#### Mods et Resource Packs
- Installation automatique des mods requis
- Gestion des mods optionnels
- Interface compacte et responsive

## ⚙️ Configuration

### Fichiers de configuration
- **Windows:** `%APPDATA%/MakeCraftRP-Launcher/`
- **macOS:** `~/Library/Application Support/MakeCraftRP-Launcher/`
- **Linux:** `~/.config/MakeCraftRP-Launcher/`

### Paramètres avancés
```json
{
  "memory": {
    "min": "2G",
    "max": "6G"
  },
  "java": {
    "path": "auto",
    "args": ["-XX:+UseG1GC", "-XX:+UnlockExperimentalVMOptions"]
  },
  "launcher": {
    "closeOnGameStart": true,
    "autoUpdate": true
  }
}
```

## 🛠️ Développement

### Structure du projet
```
MakeCraftRP-Launcher/
├── src/
│   ├── app.js              # Point d'entrée Electron
│   ├── index.html          # Page principale
│   ├── panels/             # Interfaces utilisateur
│   │   ├── home.html       # Page d'accueil
│   │   ├── settings.html   # Paramètres
│   │   └── login.html      # Connexion
│   └── assets/             # Ressources
│       ├── css/            # Styles
│       ├── js/             # Scripts
│       └── images/         # Images
├── build.js                # Script de compilation
└── package.json           # Dépendances
```

### Technologies utilisées
- **[Electron](https://electronjs.org/)** - Framework desktop
- **[minecraft-java-core](https://github.com/Luuxis/minecraft-java-core)** - Gestion Minecraft
- **[electron-updater](https://github.com/electron-userland/electron-updater)** - Mises à jour auto
- **CSS moderne** - Glassmorphism, flexbox, animations

### Scripts de développement
```bash
npm start          # Lancer en mode dev
npm run build      # Compiler pour production
npm run dev        # Mode dev avec hot-reload
```

## 🤝 Contribution

Les contributions sont les bienvenues ! Pour contribuer :

1. **Fork** le projet
2. Créez une **branche** pour votre fonctionnalité (`git checkout -b feature/AmazingFeature`)
3. **Committez** vos changements (`git commit -m 'Add: Amazing Feature'`)
4. **Push** vers la branche (`git push origin feature/AmazingFeature`)
5. Ouvrez une **Pull Request**

### Guidelines de contribution
- Suivez les conventions de code existantes
- Testez vos modifications sur plusieurs OS
- Documentez les nouvelles fonctionnalités
- Respectez le design système en place

## 📝 Changelog

### [2.2.8] - 2025-09-13
- ✨ Interface skin épurée avec preview 3D
- 🔧 Amélioration responsive des paramètres mods
- 🎨 Repositionnement du bouton paramètres
- 🐛 Corrections diverses d'interface

### [2.2.7] - 2025-09-01
- 🚀 Optimisations performance
- 📱 Améliorations responsive
- 🔄 Système de mise à jour amélioré

[Voir le changelog complet](CHANGELOG.md)

## 🐛 Problèmes connus

- **Java 21+** : Certaines versions récentes peuvent causer des problèmes
- **Antivirus** : Possibles faux positifs lors de l'installation
- **macOS** : Nécessite d'autoriser l'app dans Sécurité & Confidentialité

## 💬 Support

Besoin d'aide ? Plusieurs options s'offrent à vous :

- 📞 **Discord** : [Rejoindre le serveur](https://discord.gg/HMEMeeMkr8)
- 🐛 **Issues GitHub** : [Signaler un problème](https://github.com/MakeCraftRP/MakeCraftRP-Launcher/issues)
- 🌐 **Site web** : [makecraftrp.com](https://makecraftrp.com/)
- 📧 **Email** : contact@makecraftrp.com

## 📄 License

Ce projet est sous licence **CC0** - voir le fichier [LICENSE.md](LICENSE.md) pour plus de détails.

## 🙏 Remerciements

- **[Luuxis](https://github.com/Luuxis)** pour minecraft-java-core
- **L'équipe MakeCraftRP** pour le serveur et la communauté
- **Contributeurs** qui améliorent le launcher

---

<div align="center">

**Fait avec ❤️ par l'équipe MakeCraftRP**

[🌟 Star ce projet](https://github.com/MakeCraftRP/MakeCraftRP-Launcher) • [🐦 Twitter](https://twitter.com/makecraftrp) • [📺 YouTube](https://youtube.com/makecraftrp)

</div>
