# 🧠 Documentation Technique

## 📌 Objectif du Projet

Créer une **interface intelligente et décentralisée** permettant :

* La **lecture simplifiée de smart contracts** pour les utilisateurs non techniques.
* Un **agent personnel IA décentralisé**, contextualisé, capable d’accompagner l’utilisateur dans ses objectifs, préférences, et tâches quotidiennes.
* Une **base de connaissance personnelle** construite autour de concepts clés (Atom, Triplet, Signal).
* Une **expérience utilisateur enrichie** : organisation, planification, recommandation, journalisation et visualisation.

---

## 🧱 Concepts Fondamentaux

### 🔹 Atom

> **Unité fondamentale de connaissance enrichie de contexte.**

* Composants : `Sujet – Prédicat – Objet` + métadonnées (lieu, temps, auteur…)
* Atoms sont créés dynamiquement selon l’interaction utilisateur
* Structure :

  ```ts
  {
    name: string;
    description: string;
    createdAt: Date;
    createdBy: string;
    pictureUrl?: string;
    link?: string;
  }
  ```

### 🔹 Triplet

> **Structure sémantique minimale : `Sujet – Prédicat – Objet`.**

* Sert à construire une base de connaissance (subjective ou factuelle)
* Publics, privés ou partagés
* Exemple : `Maxime – aime – la musique électronique`

### 🔹 Signal

> **Activation d’un ou plusieurs Atoms dans un contexte donné.**

* Associé à une intention : recommandation, validation, action…
* Signal = **unité monétisable**, pouvant être lié à un **vote avec dépôt ETH**
* Permet de **pondérer la valeur d’un triplet**

---

##  1️⃣ ElizaOS = Cœur de la couche Orchestration
Dans ton projet, ElizaOS jouera le rôle de :
🎛️ Router de contexte : Il récupère tes Atoms, Triplets, Signaux et les reformate.
🧠 Prompt Engine : Il prépare les prompts pour le LLM, en intégrant contexte + requête utilisateur.
🔗 Pont entre tes LLM, ton backend Node et Intuition.system : Plus tard, tu pourras remplacer le LLM local par un agent Intuition pour la certification + micro-certification des flux.

---

🔗 2️⃣ Connexion API
En pratique :
Frontend React 👉 appelle ton backend Node
Ton backend Node 👉 appelle ElizaOS
ElizaOS 👉 appelle le LLM que tu veux (OpenAI, Ollama local, ou futur Intuition LLM).

---

## 🔐 Authentification / Connexion Web3

* Authentification via **Metamask** (cf. [wagmi.sh](https://wagmi.sh/react/getting-started))
* Connexion Wallet : [faucet dapp starter](https://github.com/jspruance/faucet-dapp-starter-code-connect-wallet)
* Intégration avec les API Google Maps et Meta Events

---

## 🧪 Fonctionnalités Clés & IA

* Intégration de **ELYSA AI** pour agir comme agent personnalisé :

  * Journalisation intelligente
  * Recommandations basées sur objectifs et dépenses
  * Génération automatique d’**Atoms certifiés** via consommation web
* Interaction avec l’extension Chrome : [Intuition Extension](https://github.com/0xIntuition/chrome-extension/)
* Base technique IA : [elizaOS/eliza](https://github.com/elizaOS/eliza), [elizaos.ai](https://www.elizaos.ai/)

---

## 💡 UX / UI

### Composants & Frameworks

* UI : [Chakra UI](https://chakra-ui.com/), [Shadcn UI](https://ui.shadcn.com/)
* Graphismes/Animations : [Spline 3D](https://spline.design/)
* Modèles 3D (avatars, personnages) : via [Sketchfab](https://sketchfab.com)

### Interaction Utilisateur

* Système de feedback : emoji, sliders, votes
* Visualisation : grid, carte géographique, favoris
* Suggestions & promotions personnalisées via préférences utilisateurs
* Interaction géolocalisée + validation d’activités IRL

---

## 🌐 Technologies Utilisées

* **GraphQL** pour les API principales
* Intégration Web avec `intuition-ts` : [GitHub](https://github.com/0xIntuition/intuition-ts)
* Extension navigateur (Chrome) : [Intuition Extension](https://github.com/0xIntuition/chrome-extension/)
* Site écosystème : [intuition.systems/ecosystem](https://www.intuition.systems/ecosystem)

---

## 🧭 Positionnement Produit & User Stories

* Ciblage initial : utilisateurs **web3 / tech** pour collecter rapidement des données certifiées
* Valeur claire à démontrer dès le MVP
* Spécificité des user stories essentielle :

  * Définir les **cercles d’usage**
  * Identifier des **centres d’intérêt prioritaires** (hors web3 aussi)
  * Définir des **cas d’usage démontrables rapidement**

---

## 💰 Économie & Monétisation

* Création des Atoms & Triplets : **gratuite**
* Activation par **Signal = mécanisme monétisable** via dépôt ETH
* Pondération possible via :

  * Engagement utilisateur (ETH investi)
  * Pertinence selon contexte et profil

---

## 🔗 Liens & Ressources Complémentaires

* Intégrations / Références :

  * [masa.ai](https://www.masa.ai/)
  * [developer.shiza.ai](https://developer.shiza.ai/exchange)
  * [world.org](https://world.org/fr-fr)
  * 

