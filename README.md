Application de bureau moderne et ultra-légère permettant d'automatiser le remplacement de têtes sur des photos de groupe pour créer des memes entre amis. Conçue pour remplacer les manipulations fastidieuses sur Photoshop sans recourir à des modèles d'IA lourds ou payants.

---

## Fonctionnalités

* **Détection faciale robuste (YuNet) :** Détecte les visages même de profil, penchés ou en arrière-plan avec estimation précise de la rotation via la position des yeux.
* **Gestion automatique et manuelle de la profondeur :** 
  * Algorithme d'ordonnancement automatique (les têtes les plus petites sont placées en arrière-plan).
  * Réorganisation manuelle des calques (*Premier plan*, *Arrière-plan*, *Monter*, *Descendre*).
* **Interface graphique CustomTkinter :** Thème sombre élégant, curseurs interactifs et prévisualisation instantanée.
* **Interaction à la souris :**
  * Glisser-déposer direct (*Drag & Drop*) pour déplacer les visages.
  * Molette de la souris pour agrandir ou réduire à la volée.
  * Clic dans le vide pour ajouter un visage manquant (personne de dos, déguisement, etc.).
* **Finition propre :**
  * Harmonisation colorimétrique automatique (espace colorimétrique LAB).
  * Adoucissement des contours du masque alpha (*feathering*) pour éviter l'effet découpe nette.
* **Export haute fidélité :** Rendu final exporté à la résolution native de la photo source (PNG ou JPEG).

---

## Technologies & Prérequis

* **Python 3.8+**
* **Bibliothèques :**
  * `customtkinter` (Interface graphique moderne)
  * `opencv-python` (Traitement d'image & détection faciale YuNet)
  * `pillow` (Manipulation d'images avec transparence RGBA)
  * `numpy` (Calculs matriciels)

> **Zéro dépendance lourde :** Aucun GPU, ni PyTorch/TensorFlow n'est nécessaire. Le modèle officiel OpenCV YuNet (~230 Ko) est téléchargé automatiquement au premier démarrage.

---

## Installation

1. **Telecharger la derniere version**
