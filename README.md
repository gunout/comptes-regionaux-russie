# 🇷🇺 Comptes régionaux Russie · Dashboard interactif

Dashboard d'analyse budgétaire des 89 sujets fédéraux russes. Comparaison multi-régions, carte interactive, analyse de soutenabilité (DSA), clusters économétriques, méthodologie académique et mode Classroom.

[![Licence MIT](https://img.shields.io/badge/Licence-MIT-ED2939?style=for-the-badge)](LICENSE)
[![Made in France](https://img.shields.io/badge/Made_in-France-002395?style=for-the-badge&labelColor=FFFFFF&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCA5MDAgNjAwIj48cmVjdCB3aWR0aD0iOTAwIiBoZWlnaHQ9IjYwMCIgZmlsbD0iIzAwMjM5NSIvPjxyZWN0IHdpZHRoPSI5MDAiIGhlaWdodD0iNDAwIiB5PSIxMDAiIGZpbGw9IiNmZmYiLz48cmVjdCB3aWR0aD0iOTAwIiBoZWlnaHQ9IjIwMCIgeT0iNDAwIiBmaWxsPSIjZWQyOTM5Ii8+PC9zdmc+)](https://github.com/gunout)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)](https://github.com/gunout/comptes-regionaux-russie)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)](https://github.com/gunout/comptes-regionaux-russie)
[![Chart.js](https://img.shields.io/badge/Chart.js-4.4-FF6384?style=flat-square&logo=chartdotjs&logoColor=white)](https://www.chartjs.org/)
[![GitHub Pages](https://img.shields.io/badge/GitHub_Pages-en_ligne-222?style=flat-square&logo=githubpages&logoColor=white)](https://gunout.github.io/comptes-regionaux-russie/)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen?style=flat-square)](https://github.com/gunout/comptes-regionaux-russie/pulls)
[![Open Data](https://img.shields.io/badge/Open_Data-Roskazna_Minfin-ff6f00?style=flat-square)](https://roskazna.gov.ru)
[![Domar](https://img.shields.io/badge/Mod%C3%A8le-Domar_%C3%A9tendu-0055A4?style=flat-square)](https://en.wikipedia.org/wiki/Domar_model)
[![DSA](https://img.shields.io/badge/Analyse-DSA_FMI-8B5CF6?style=flat-square)](https://www.imf.org)
[![SpVAR](https://img.shields.io/badge/SpVAR-Banque_de_Russie-10B981?style=flat-square)](https://cbr.ru)

---

## 📑 Sommaire

- [Aperçu](#-aperçu)
- [Fonctionnalités](#-fonctionnalités)
- [Démo](#-démo)
- [Installation](#-installation)
- [Déploiement GitHub Pages](#-déploiement-github-pages)
- [Contenu du dashboard](#-contenu-du-dashboard)
- [Données](#-données)
- [Méthodologie](#-méthodologie)
- [Structure du projet](#-structure-du-projet)
- [Exports](#-exports)
- [Limitations](#-limitations)
- [Références académiques](#-références-académiques)
- [Licence](#-licence)

---

## 🔎 Aperçu

Un fichier HTML unique, sans build ni dépendance npm, qui implémente un **dashboard interactif d'analyse des comptes budgétaires des 89 sujets fédéraux russes**. L'outil combine visualisation interactive, comparaison multi-régions, analyse de soutenabilité de la dette et contenu pédagogique pour étudiants en économie.

L'application est **100 % côté client** : aucune donnée n'est envoyée à un serveur, aucun compte n'est requis, aucune dépendance externe n'est installée.

> ⚠️ **Outil académique et pédagogique** — Ne constitue pas un conseil en investissement ni une analyse officielle.

---

## ✨ Fonctionnalités

### 📊 7 onglets principaux

1. **Vue d'ensemble** — KPI globaux, évolution historique 2015-2025, top 10 dette, contexte historique
2. **Comparaison** — Sélection de 2 à 15 régions, 7 analyses comparatives
3. **Carte interactive** — Visualisation des 89 régions avec code couleur par dette
4. **Soutenabilité** — KPI DSA, nuage VFI × Soutenabilité, matrice pb* × (r−g)
5. **Données** — Tableau détaillé triable (12 colonnes)
6. **Méthodologie** — Domar, VFI, structure dette, sources, bibliographie
7. **Classroom** — 4 exercices guidés pour étudiants

### 🎯 Analyse comparative (7 vues)

- **Barres comparatives** — Recettes, dépenses, dette côte à côte
- **Radar** — Profils normalisés sur 6 axes
- **Séries temporelles** — Évolution 2015-2025
- **Scatter VFI × Soutenabilité** — Nuage des 89 régions + sélection
- **Structure de la dette** — ОФЗ / Crédits bancaires / Prêts budgétaires / Garanties
- **Agrégats par district** — Comparaison inter-districts fédéraux
- **Clusters** — 5 groupes identifiés par k-means

### 🗺️ Carte interactive

- Représentation SVG des 89 régions
- Code couleur selon la dette : 🟢 < 50 Md₽ · 🟡 50-100 · 🔴 100-200 · 🔴🔴 > 200
- Clic pour sélectionner/désélectionner une région
- Synchronisation avec les autres onglets

### ⚖️ Analyse de soutenabilité (DSA)

- Indicateur composite de soutenabilité (0-100)
- Trois ratios : Dette/GRP, Dette/Recettes, VFI
- Relation inverse VFI ↔ soutenabilité
- Matrice de sensibilité pb* × (r−g)

### 🎨 Interface

- **Thème clair/sombre** avec bascule automatique
- **URL state** — Bouton 🔗 pour partager une vue
- **Deep linking** — Restauration de l'état via paramètres URL
- **Responsive** — Adapté mobile, tablette, desktop
- **Sections repliables**
- **5 boutons de sélection rapide** : Tout, Aucun, Top 10 dette, Donatrices, Risque élevé

---

## 🚀 Démo

### 🌐 Application en ligne

👉 [**https://gunout.github.io/comptes-regionaux-russie/**](https://gunout.github.io/comptes-regionaux-russie/)

Aucune installation, aucune inscription. Ouvrez le lien dans un navigateur moderne.

---

## 📦 Installation

### Utilisation directe (recommandée)

```bash
git clone https://github.com/gunout/comptes-regionaux-russie.git
cd comptes-regionaux-russie
# Ouvrez index.html dans votre navigateur
```

Aucune dépendance, aucun `npm install`, aucun build.

### Serveur local (optionnel)

```bash
# Python 3
python -m http.server 8000

# ou Node.js
npx serve .
```

Puis ouvrez `http://localhost:8000/index.html`.

---

## 🌐 Déploiement GitHub Pages

L'application est **déjà déployée** à l'adresse :

**🔗 [https://gunout.github.io/comptes-regionaux-russie/](https://gunout.github.io/comptes-regionaux-russie/)**

### Déployer sur votre propre fork

1. **Forkez** le dépôt sur GitHub
2. Le fichier `index.html` doit être **à la racine** du dépôt
3. Allez dans **Settings → Pages**
4. Sous **Build and deployment** :
   - **Source** : `Deploy from a branch`
   - **Branch** : `main` / `(root)`
5. Cliquez sur **Save**
6. Attendez 1-2 minutes

Votre site sera accessible à :
`https://<votre-compte>.github.io/<votre-repo>/`

### Ajouter un fichier `.nojekyll`

Pour éviter tout traitement Jekyll inutile :

```bash
touch .nojekyll
git add .nojekyll
git commit -m "chore: add .nojekyll"
git push
```

---

## 📋 Contenu du dashboard

### KPI globaux

| Indicateur | Valeur 2025 |
|---|---|
| Recettes totales | 25 858 Md₽ |
| Dépenses totales | 27 397 Md₽ |
| Solde consolidé | −1 538 Md₽ |
| Dette totale | 3 481 Md₽ |
| Régions déficitaires | 74 / 89 |
| Régions donatrices | 22 / 89 |
| VFI moyen | 34% |
| Soutenabilité moyenne | 62 / 100 |

### 9 districts fédéraux

| Code | District | Régions |
|---|---|---|
| **CFO** | Central | 18 |
| **SZFO** | Nord-Ouest | 11 |
| **YFO** | Sud | 8 |
| **SKFO** | Caucase Nord | 7 |
| **PFO** | Volga | 14 |
| **UFO** | Oural | 6 |
| **SFO** | Sibérie | 10 |
| **DFO** | Extrême-Orient | 11 |
| **NEW** | Nouveaux territoires | 4 |

### 5 clusters identifiés

- 🟢 **Leaders autonomes** — Moscou, SPb, Tatarstan, Khanty-Mansi, Yamalo-Nenets, Sakhalin, Tyumen
- 🔵 **Industrielles robustes** — Sverdlovsk, Chelyabinsk, Krasnoyarsk, Kemerovo, Irkoutsk, Perm, Samara, Bashkortostan
- 🟡 **En transition** — Krasnodar, Rostov, Nijni Novgorod, Novossibirsk, Voronezh, Volgograd
- 🔴 **Dépendantes** — Daghestan, Tchétchénie, Ingouchie, Tyva, Kalmykie, Kabardino-Balkarie
- ⚫ **Nouveaux territoires** — Donetsk, Lougansk, Zaporijjia, Kherson

---

## 📊 Données

### Sources officielles

| Source | Contenu | Accès |
|---|---|---|
| **Roskazna** | Trésor fédéral, exécution budgétaire | [roskazna.gov.ru](https://roskazna.gov.ru) |
| **Minfin Russia** | Dette publique régionale | [minfin.gov.ru](https://minfin.gov.ru) |
| **ACRA Ratings** | Notations et structure des recettes | [acra-ratings.ru](https://www.acra-ratings.ru) |
| **Banque de Russie** | Multiplicateurs budgétaires (WP 138) | [cbr.ru](https://www.cbr.ru) |
| **ЕМИСС / fedstat.ru** | Recettes des budgets consolidés | [fedstat.ru](https://www.fedstat.ru) |
| **HSE** | Recherche académique sur la convergence spatiale | [hse.ru](https://www.hse.ru) |
| **budget.gov.ru** | Portail unifié du système budgétaire | [budget.gov.ru](https://budget.gov.ru) |

### Champs extraits par région

| Champ | Description |
|---|---|
| `name` | Nom du sujet fédéral |
| `district` | District fédéral (CFO, SZFO, …) |
| `grp` | Produit régional brut (Md₽) |
| `pop` | Population (milliers) |
| `rev2025` | Recettes 2025 (Md₽) |
| `exp2025` | Dépenses 2025 (Md₽) |
| `debt` | Encours de dette (Md₽) |
| `vfi` | Déséquilibre Budgétaire Vertical (%) |
| `sustain` | Indice de soutenabilité (0-100) |
| `donator` | Région donatrice nette (booléen) |
| `instruments` | Répartition ОФЗ / banque / budget / garanties |

---

## 📐 Méthodologie

### Équation de Domar

Le dashboard utilise l'équation de Domar discrète pour analyser la dynamique de la dette :

```
Δb_t = [(r_t − g_t) / (1 + g_t)] · b_{t−1} − pb_t / (1 + g_t)
```

Où :
- `b` = dette / PIB (ou dette / GRP au niveau régional)
- `r` = taux d'intérêt effectif
- `g` = croissance nominale
- `pb` = solde primaire (% PIB)

### Solde primaire stabilisant

```
pb* = [(r − g) / (1 + g)] · b
```

### Déséquilibre Budgétaire Vertical (VFI)

```
VFI = Transferts fédéraux / Recettes totales × 100
```

Interprétation :
- VFI < 30% : région autonome (donatrice nette)
- VFI 30-60% : dépendance modérée
- VFI > 60% : dépendance forte aux transferts

### Indice de soutenabilité

Indice composite (0-100) combinant :
- Dette / GRP (poids 40%)
- Dette / Recettes (poids 40%)
- Inverse du VFI (poids 20%)

---

## 📁 Structure du projet

```text
.
├── index.html      # Application complète (HTML + CSS + JS inline)
├── README.md       # Ce fichier
├── LICENSE         # MIT
└── .nojekyll       # (optionnel) désactive Jekyll sur GitHub Pages
```

L'application est volontairement monolithique pour faciliter le déploiement et l'audit.

---

## 📥 Exports

| Format | Contenu |
|---|---|
| **CSV** | Tableau complet des 89 régions (12 colonnes) |
| **JSON** | Données structurées réutilisables |
| **Excel** | Tableau détaillé (.xls) |
| **PDF** | Rapport complet (KPI + tableau + sélection) |
| **API JSON** | Point d'accès statique pour réutilisation par d'autres chercheurs |

---

## ⚠️ Limitations

- **Données statiques** : les valeurs sont calibrées sur les ordres de grandeur connus, mais ne sont pas mises à jour automatiquement
- **Pas de connexion API en temps réel** : les données sont codées en dur
- **Modèle simplifié** : pas de réaction endogène de la politique budgétaire
- **Pas de modélisation VAR** : les multiplicateurs budgétaires ne sont pas calculés en direct
- **Carte simplifiée** : la représentation SVG utilise une grille et non une vraie projection géographique
- **Nouveaux territoires** : les données sont indicatives et non officielles

---

## 📚 Références académiques

- **Domar, E. D.** (1944), *The "Burden of the Debt" and the National Income*, American Economic Review
- **Blanchard, O.** (2019), *Public Debt and Low Interest Rates*, American Economic Review
- **FMI** (2022), *Staff Guidance Note on the Sovereign Risk and Debt Sustainability Framework*
- **Banque de Russie** (2024), *Regional finance and fiscal regulation: estimating fiscal multiplier*, Working Paper Series No. 138
- **Timushev, E. N. & Mikhaylova, A. A.** (2023), *Vertical fiscal imbalance as a tool for analyzing the debt sustainability of Russian regions*, State and Municipal Management Scholar Notes
- **Lavrovskii, B. L. & Goryushkina, E. A.** (2025), *Equalization of fiscal capacity in Russian regions: Illusion or reality?*, Voprosy Ekonomiki
- **Mykalo, R.** (2026), *Assessment of the Impact of Budget Policy Shocks on the Economy of Russian Regions*, HSE Master's Thesis
- **Lishnevkiy, A.** (2025), *Estimation of the Size and Administrative-Territorial Division Impact on the Efficiency of Government Spending in Regions of the Russian Federation*, HSE Master's Thesis

---

## 🎓 Mode Classroom

Le dashboard inclut 4 exercices guidés pour étudiants en économie :

1. **Comprendre le VFI** — Comparer les régions du Caucase Nord aux régions donatrices
2. **Effet boule de neige** — Simuler r − g positif et négatif
3. **Comparaison de clusters** — Observer les 4 groupes identifiés automatiquement
4. **Structure de la dette** — Comparer ОФЗ / crédits bancaires / prêts budgétaires

---

## 📄 Licence

Ce projet est distribué sous licence **MIT** — voir le fichier [LICENSE](LICENSE) pour plus de détails.

```text
MIT License

Copyright (c) 2026 gunout

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

---

## 🙏 Remerciements

- **Roskazna** — Trésor fédéral russe, données d'exécution budgétaire
- **Minfin Russia** — Ministère des Finances, données de dette
- **ACRA Ratings** — Notations régionales et structure des recettes
- **Banque de Russie** — Recherche sur les multiplicateurs budgétaires
- **HSE** — Recherche académique sur la convergence spatiale
- **ЕМИСС / fedstat.ru** — Données budgétaires consolidées

---

<div align="center">

**📊 Outil académique — Ne constitue pas un conseil en investissement**

Fait pour la communauté économique open source.

</div>

---

<div align="center">

### 🇫🇷 Gunout · 2026

![Made in France](https://img.shields.io/badge/Made_in-France-002395?style=flat-square&labelColor=FFFFFF&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCA5MDAgNjAwIj48cmVjdCB3aWR0aD0iOTAwIiBoZWlnaHQ9IjYwMCIgZmlsbD0iIzAwMjM5NSIvPjxyZWN0IHdpZHRoPSI5MDAiIGhlaWdodD0iNDAwIiB5PSIxMDAiIGZpbGw9IiNmZmYiLz48cmVjdCB3aWR0aD0iOTAwIiBoZWlnaHQ9IjIwMCIgeT0iNDAwIiBmaWxsPSIjZWQyOTM5Ii8+PC9zdmc+)
![GitHub](https://img.shields.io/badge/GitHub-gunout-181717?style=flat-square&logo=github&logoColor=white)
![Year](https://img.shields.io/badge/2026-ED2939?style=flat-square&labelColor=FFFFFF)

<sub>© 2026 <strong>gunout</strong> — Tous droits réservés.</sub>

</div>
