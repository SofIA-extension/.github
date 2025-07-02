
# 🧠 SOFIA — Agent IA Personnel pour le Web

> **SOFIA** est une extension Chrome dopée à l’intelligence artificielle, pensée comme un agent personnel intelligent.

---

## ✨ Présentation

**SOFIA** t’accompagne dans ta navigation web, capte tes centres d’intérêt et les transforme en une **mémoire numérique vivante**, **sécurisée** et **vérifiable via la blockchain**.

Mais elle ne fait pas que t’assister :
- Elle **structure, contextualise et certifie** ton identité numérique.
- Grâce à l’infrastructure décentralisée d’[Intuition.systems](https://www.intuition.systems/), chaque interaction peut devenir un **atom**, une unité de connaissance.
- Tu choisis si ces données restent **privées**, **partagées**, ou **ancrées on-chain**.

🧭 **SOFIA** agit comme :
- Un **journal assisté**
- Un **graphe personnel vivant**
- Un **planificateur intelligent**
- Un **filtre cognitif**
- Un **complice éthique** de ta mémoire numérique

---

## 🧰 Stack Technique

| Élément        | Version       |
|----------------|---------------|
| Node.js        | v20.19.3      |
| pnpm           | v10.8.2       |
| Vite           | v7.0.0        |
| Framework UI   | [Chakra UI](https://chakra-ui.com/) / [Shadcn UI](https://ui.shadcn.com/) |
| Auth           | MetaMask / Wagmi |
| API            | Google Maps, Intuition.systems |
| Extension      | Chrome |
| Web3           | Intégration on-chain via signaux/atoms/triplets |
| Langage        | TypeScript    |

---

## 🗂️ Structure recommandée du dépôt

```bash
sofia/
├── main             # Branche de production (stable)
├── develop          # Branche de développement
├── feature/         # Branches de fonctionnalités
│   ├── feature/chatbot
│   ├── feature/onboarding
├── bugfix/          # Branches de correction
├── hotfix/          # Correctifs urgents en prod
├── README.md        # Présentation du projet
├── docs/            # Documentation complémentaire
├── .github/         # Workflows CI/CD, templates d’issues/PR
└── LICENSE          # Licence open source
```

---

## 🌳 Convention Git

### 🛠 Branches

- `main` : version en production
- `develop` : branche de dev continue (version testée mais non prod)
- `feature/xxx` : nouvelles fonctionnalités
- `bugfix/xxx` : correction de bugs
- `hotfix/xxx` : correctifs urgents en production

### 🔄 Workflow Git

1. Développement sur `feature/xxx`
2. Merge vers `develop` après tests
3. Merge vers `main` pour release
4. `hotfix/xxx` part de `main` et merge vers `main` + `develop`

### 🔐 Protection des branches

> GitHub → Settings → Branches → Protection rules

- 🔒 Interdiction des push directs sur `main` et `develop`
- ✅ Revue obligatoire via Pull Request
- ✅ (Optionnel) Intégration continue obligatoire pour valider les PRs

---

## 🤝 Contribution

Avant de contribuer :

1. Fork le projet
2. Crée une branche depuis `develop` :
   ```bash
   git checkout -b feature/nom-fonctionnalité
   ```
3. Push ta branche :
   ```bash
   git push origin feature/nom-fonctionnalité
   ```
4. Ouvre une Pull Request vers `develop`

Merci de respecter :
- La convention de commit (`feat:`, `fix:`, `docs:`, etc.)
- Les bonnes pratiques d'accessibilité et de lisibilité
- Les standards TypeScript / Vite

---

## 📌 TODO (Roadmap Initiale)

- [ ] Intégration complète avec Intuition.systems (atoms/triplets/signaux)
- [ ] Interface de visualisation des centres d’intérêt
- [ ] Fonction de journal assisté avec classification automatique
- [ ] Détection automatique d’actions/contextes dans le navigateur
- [ ] Mode privé / public pour chaque interaction
- [ ] Onboarding UX avec personnalisation de l’agent IA
- [ ] Détection de "moments à retenir"
- [ ] Intégration Google Maps (activités à proximité)
- [ ] Mécanisme de vote ou réaction aux triplets (signaux)
- [ ] Interface Web3 / Wallet / ETH staking sur signaux
- [ ] Version décentralisée des favoris, objectifs, rappels

---

## 🔗 Ressources externes

- Intuition System : [intuition-ts](https://github.com/0xIntuition/intuition-ts)
- Eliza OS : [GitHub](https://github.com/elizaOS/eliza) – [Site](https://www.elizaos.ai/)
- Extension Chrome : [Intuition Extension](https://github.com/0xIntuition/chrome-extension)
- Metamask Auth : [wagmi.sh](https://wagmi.sh/react/getting-started)

---

## ⚖️ Licence

Ce projet est sous licence MIT. Voir le fichier [LICENSE](./LICENSE).
