# STM32 Development Board V1.1

Une carte de développement professionnelle basée sur le microcontrôleur **STM32G431VBT6**, dotée de multiples GPIO, deux connecteurs USB-C et deux oscillateurs cristal pour les applications nécessitant une synchronisation précise.

## 📋 Aperçu

![Vue 3D Isométrique](images/3d_isometric.png)

Cette carte de développement est conçue comme une plateforme polyvalente pour le développement de systèmes embarqués, les applications IoT et le prototypage de microcontrôleurs. Le STM32G431VBT6 est un processeur ARM Cortex-M4 puissant tournant à jusqu'à 170 MHz.

## ✨ Caractéristiques Principales

### Microcontrôleur
- **Processeur** : STM32G431VBT6 (ARM Cortex-M4)
- **Vitesse** : Jusqu'à 170 MHz
- **Mémoire Flash** : 256 KB
- **RAM** : 36 KB
- **Boîtier** : LQFP100

### Connectivité & Alimentation
- **Deux connecteurs USB-C** - Options de connectivité multiples et livraison d'énergie
- **Multiples broches GPIO** - Options d'entrée/sortie étendues pour capteurs et périphériques
- **Deux oscillateurs cristal** - Pour une synchronisation précise et la redondance

### Conception Physique
- **Dimensions** : Optimisées pour la compatibilité breadboard et prototypage
- **Arrangement des GPIO** : Connecteurs organisés sur les côtés gauche et droit pour un accès facile
- **Fixation** : Quatre trous de montage (visibles dans la vue 3D)

## 🎨 Design du PCB

### Vue du Dessus - Couche Routage Rouge
![PCB Dessus - Couche Rouge](images/pcb_top_red.png)

La couche primaire de routage des signaux montrant les interconnexions principales entre les composants, la distribution d'énergie et les chemins de signaux.

### Vue du Dessus - Couche Routage Bleu
![PCB Dessus - Couche Bleue](images/pcb_top_blue.png)

La couche secondaire de routage illustrant le réseau complet de distribution des signaux et de l'alimentation à travers la carte.

## 📊 Diagramme Fonctionnel

```
┌──────────────────────────────────────────┐
│     STM32G431VBT6 (Cortex-M4)           │
│        170 MHz, 256KB Flash             │
└──────────────────────────────────────────┘
           │
    ┌──────┼──────┐
    │      │      │
    ▼      ▼      ▼
┌────────┐ ┌────────┐ ┌────────┐
│ USB-C  │ │ GPIO   │ │Cristaux│
│Port 1  │ │Expands.│ │ Dual  │
├────────┤ ├────────┤ ├────────┤
│USB-C   │ │        │ │ 8-32MHz│
│Port 2  │ │ 80 pins│ │ (x2)  │
└────────┘ └────────┘ └────────┘
    │      │      │
    └──────┬──────┘
           │
    ┌──────▼──────┐
    │  GPIO I/O   │
    │ (80 broches)│
    └─────────────┘
```

## 📌 Configuration des Broches

La carte comprend **80 broches GPIO** arrangées comme suit :
- **40 broches par côté** (Gauche et Droite)
- **Étiquetées pour une identification facile**
- **Support des fonctions analogique et numérique**

## 💡 Applications

- 🔌 **Appareils IoT** - Capteurs connectés et surveillance à distance
- 🤖 **Robotique** - Contrôle moteur et intégration de capteurs
- 📊 **Acquisition de Données** - Applications ADC multi-canaux et critiques en timing
- 🔬 **Prototypage** - Développement rapide de systèmes embarqués
- ⚡ **Gestion d'Énergie** - Conversion CC-CC efficace et livraison d'énergie

## 🚀 Démarrage Rapide

### Outils Requis
- STM32CubeIDE ou ARM MDK
- Déboguer ST-LINK V2 (ou compatible)
- Câble USB-C
- Bibliothèques ST appropriées

### Configuration de Base
1. Connectez le déboguer ST-LINK à la carte
2. Connectez l'USB-C pour l'alimentation et la communication
3. Flashez votre firmware en utilisant STM32CubeProgrammer
4. Commencez à développer !

## 📚 Documentation

| Resource | Lien |
|----------|------|
| **Feuille de données microcontrôleur** | [STM32G431 Datasheet](https://www.st.com/resource/en/datasheet/stm32g431vb.pdf) |
| **Environnement de développement** | [STM32CubeIDE](https://www.st.com/en/development-tools/stm32cubeide.html) |
| **Programmeur** | [STM32CubeProgrammer](https://www.st.com/en/development-tools/stm32cubeprog.html) |

## 🔧 Spécifications Matérielles

| Spécification | Valeur |
|---------------|--------|
| **Cœur** | ARM Cortex-M4 |
| **Vitesse d'horloge** | 170 MHz |
| **Mémoire Flash** | 256 KB |
| **SRAM** | 36 KB |
| **Broches GPIO** | 80 |
| **Canaux ADC** | Multiples |
| **Minuteurs** | Multiples (16/32-bit) |
| **UART/USART** | Multiples |
| **SPI/I2C** | Multiples |
| **USB** | 2x USB-C |
| **Cristaux** | 2x (Support oscillateur dual) |

## 📁 Structure du Dépôt

```
STM32_DEVBOARD_V1.1/
├── Hardware/
│   ├── PCB/
│   │   ├── STM32_DEVBOARD.PcbDoc
│   │   ├── STM32_DEVBOARD.SchDoc
│   │   └── Gerbers.zip
│   ├── Images/
│   │   ├── PCB_Top.png
│   │   ├── PCB_Bottom.png
│   │   └── PCB_3D.png
│   └── README.md
├── images/
│   ├── 3d_isometric.png
│   ├── pcb_top_red.png
│   └── pcb_top_blue.png
└── README.md
```

## 📈 État du Projet

- ✅ Design PCB Complété
- ✅ Vérification de la Mise en Page
- 🔄 Phase de Fabrication
- ⏳ Test & Validation (À venir)

## 📝 License

Ce projet est licencié sous la [MIT License](LICENSE) - libre d'utilisation, modification et distribution.

## 📧 Contact & Support

**Auteur** : Felix-JRDB  
**Email** : felixjeanrichard4@gmail.com  
**Repository** : https://github.com/Felix-JRDB/STM32_DEVBOARD_V1.1

Pour les problèmes, suggestions ou contributions, veuillez ouvrir une issue sur GitHub.

---

**Dernière Mise à Jour** : Juin 2026  
**Version** : 1.1
