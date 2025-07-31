# 🔐 KeyManager - Système de Clés Avancé
**KeyManager** est un plugin Minecraft conçu pour enrichir l'expérience **rôleplay** de votre serveur avec un système de sécurité immersif et réaliste. Transformez vos portes en véritables **systèmes de verrouillage** avec des **clés personnalisées**, un **mini-jeu de crochetage** captivant, et un **système de permissions sophistiqué**.

``Que vous soyez propriétaire d'une maison, invité de confiance, ou cambrioleur expérimenté, KeyManager offre une expérience unique qui renforce l'immersion et les interactions entre joueurs.``

## ✨ Fonctionnalités Principales
### 🗝️ Système de Clés Intelligent

-  **Clés vierges :** Créez et liez vos clés à n'importe quelle porte
-  **Clés de propriétaire :** Contrôle total (liaison, verrouillage, déverrouillage)
-  **Clés d'invité :** Accès et utilisation sans pouvoir créer de nouvelles liaisons
-  **Support des doubles portes :** Détection automatique et liaison simultanée
-  **Clés personnalisées :** Chaque clé affiche sa destination et son statut

### 🔓 Mini-Jeu de Crochetage

-  **Système 4/4 :** Réussissez 4 séquences consécutives pour déverrouiller
-  **Timing précis :** 0.5 seconde pour réagir au signal sonore
-  **Sons immersifs :** Séquences audio avec grincements et cliquetis
-  **Interface hotbar :** Messages d'état en temps réel
-  **Progression visuelle :** Compteur de succès (1/4, 2/4, 3/4, 4/4)
-  **Système de cooldown :** 30 secondes d'attente après échec

### 🚨 Système de Sécurité RP

-  **Alertes en temps réel :** Les propriétaires sont notifiés lors de crochetages
-  **Journal d'accès :** Historique détaillé de toutes les actions (50 dernières entrées)
-  **Notifications intelligentes :** Seuls les vrais propriétaires reçoivent les alertes
-  **Son d'alarme :** Signal sonore distinctif pour les propriétaires

### 🛠️ Outils de Crochetage

-  **Consommables :** Chaque tentative consomme un outil
-  ***Nom personnalisé :** "Outils de crochetage" avec description détaillée
-  **Usage unique :** Se casse après utilisation (succès ou échec)
-  **Craft contrôlé :** Distribution via commandes administrateur


### 🎮 Commandes Disponibles

-  ***/givekey*** *Donne une clé (vierge ou copiée)*
        `/givekey [joueur] [proprio/invite] [numéro]`
-  ***/delinkkey*** *Délie une clé de sa porte*
        `/delinkkey <numéro>`
-  ***/givecrochetage*** *Donne des outils de crochetage*
        `/givecrochetage [joueur] [nombre]horiziakeys.admin`

## 🎯 Utilisation Pratique

### Pour les Propriétaires :

-  Obtenir une clé vierge via un administrateur
-  Clic droit sur une porte pour la lier (devient automatiquement propriétaire)
-  Shift + clic droit pour verrouiller/déverrouiller
-  Recevoir des alertes en cas de tentative de crochetage

### Pour les Invités :

-  Recevoir une clé d'invité d'un administrateur (clé déjà liée)
-  Accéder librement aux portes autorisées
-  Verrouiller/déverrouiller comme un propriétaire
-  Pas d'alertes lors de crochetages (sécurité préservée)

### Pour les Cambrioleurs :

-  Obtenir des outils de crochetage via le marché noir ou administrateur
-  Clic droit sur une porte verrouillée pour commencer
-  Écouter attentivement les séquences sonores (bong bong bong bong bong BING)
-  Cliquer au bon moment sur le signal spécial
-  Répéter 4 fois sans échouer pour réussir


## 📊 Système de Données
### Journal d'Accès (keys.yml)
  **Chaque clé conserve un historique détaillé :**

``yaml``

    keys:
      "1":
        location: "world:100:64:200"
        holders:
          proprio: ["Alice", "Bob"]
          invite: ["Charlie", "Diana"]
        access_log:
          - "2024-01-15 14:30:25 - Alice - LIAISON"
          - "2024-01-15 15:45:12 - Charlie - OUVERTURE"
          - "2024-01-15 16:20:33 - Hacker123 - CROCHETAGE"
      
### Types d'Actions Enregistrées

-  **LIAISON :** *Création du lien clé-porte*
-  **VERROUILLAGE :** *Fermeture de la serrure*
-  **DÉVERROUILLAGE :** *Ouverture de la serrure*
-  **OUVERTURE :** *Passage par la porte avec clé*
-  **CROCHETAGE :** *Intrusion réussie*


## 🎨 Interface Utilisateur
### `Messages Hotbar (immersion maximale)`

-  **🔓 Crochetage en cours...**
-  **✓ Bon timing ! (2/4)**
-  **✓ Serrure crochetée avec succès !**
-  **✗ Crochetage échoué : Trop lent !**
-  **💔 Votre crochet s'est cassé !**
-  **Porte verrouillée / Double porte déverrouillée**

### `Notifications de Sécurité (chat)`

-  **⚠ ALERTE : Hacker123 a crocheté votre serrure !**
`Position: 150, 64, -75`


## 🔧 Configuration et Installation
### Compatibilité

-  **Minecraft :** 1.20.2+
-  **Plateforme :** Paper (recommandé)
-  **Langage :** Java 17+

### Permissions

``yamlpermissions:``

      horiziakeys.admin:
        description: "Accès aux commandes administrateur"
        default: op
    
### Installation

-  Télécharger le fichier .jar
-  Placer dans le dossier plugins/
-  Redémarrer le serveur
-  Le fichier keys.yml sera créé automatiquement

# Preview 

**https://youtu.be/X5hgRsEd7as**

*Si vous êtes intéressé par ce plugin Minecraft ou si vous avez la moindre question à son sujet, vous pouvez me contacter sur mon Discord* ***@t3mrn***.
