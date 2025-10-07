# 🎬 Analyse du catalogue Netflix  
### Comprendre les tendances mondiales du streaming et des contenus

> **Dataset :** Kaggle – *Netflix Movies and TV Shows* (`netflix_titles.csv`)  
> **Outils :** Power BI · Python (pandas, matplotlib, seaborn) · Excel  
> **Auteur :** [Omayma BELHASSANE] – Business Data Analyst 

---

## ❓ Problème

Netflix dispose d’un catalogue mondial (films & séries) publié dans plus de 190 pays.  
Pour piloter la **programmation**, l’**acquisition** et le **marketing**, il faut comprendre :

- les **tendances temporelles** (pics d’ajouts, montée des séries depuis 2015, etc.),  
- la **répartition géographique** (pays dominants, diversification),  
- la **typologie de contenus** (genres, classifications d’âge),  
- et comment **équilibrer** le catalogue pour **maximiser l’engagement**.

**Problématique :**  
> *Comment l’analyse du catalogue Netflix peut-elle aider à identifier les tendances clés et orienter les décisions de production, d’acquisition et de diffusion ?*

---

## 👩‍💻 Mon rôle

Rôle : **Data Analyst / BI**

**Missions clés :**
- Traduire les **questions business** en **KPI** actionnables.  
- **Nettoyer**, **structurer** et **visualiser** la donnée.  
- Construire un **dashboard Power BI** interactif.  
- Rédiger un **storytelling** clair pour décideurs non techniques.

---

## 🧩 Dataset

- **Source officielle :** [Kaggle – Netflix Movies and TV Shows](https://www.kaggle.com/datasets/shivamb/netflix-shows)  
- **Volume :** ~7 000 titres  
- **Champs clés :**  
  `type` (Movie/TV Show), `title`, `country`, `date_added`, `release_year`, `rating`, `duration`, `listed_in` (genres), `description`.

---

## ⚙️ Outils & méthodes

| Catégorie      | Détails |
|----------------|--------|
| Préparation    | Excel (aperçu), Python (pandas) |
| Analyse        | Python (pandas, matplotlib, seaborn) |
| Visualisation  | Power BI (modélisation, DAX, filtres) |
| Documentation  | Markdown (README), notebooks Jupyter |

---

# 🎯 Étape 1 — Traduire les questions business en KPI actionnables

> **Objectif :** comprendre les enjeux métiers de Netflix et définir les indicateurs clés qui guideront toute l’analyse.

---

## 💼 Contexte métier

Netflix souhaite mieux comprendre :
- L’évolution de son **catalogue** (films vs séries, genres, années, pays).  
- Les **zones géographiques** dominantes et les **marchés émergents**.  
- Les **préférences de contenu** (genre, format, rating).  
- Les leviers pour **optimiser la production et la diffusion** des contenus.

---

## 🧭 Questions business clés

1️⃣ Quels types de contenus dominent la plateforme (films ou séries) ?  
2️⃣ Quels pays produisent le plus de titres ?  
3️⃣ Quels genres sont les plus représentés ?  
4️⃣ Comment le catalogue a-t-il évolué dans le temps ?  
5️⃣ Quelle est la classification d’âge dominante (TV-MA, PG, etc.) ?  
6️⃣ Netflix se diversifie-t-il géographiquement ?  

---

## 📊 Traduction en KPI (indicateurs actionnables)

| Question métier | KPI associé | Objectif stratégique |
|-----------------|--------------|----------------------|
| Films vs Séries ? | % de films / % de séries | Identifier la stratégie de contenu |
| Top pays producteurs ? | Nombre de titres par pays | Identifier les marchés dominants |
| Genres dominants ? | Top 5 genres les plus fréquents | Comprendre les préférences du public |
| Tendance annuelle ? | Nombre de titres ajoutés par année | Suivre la croissance du catalogue |
| Public cible ? | Répartition des ratings (TV-MA, PG...) | Adapter les campagnes marketing |
| Diversité géographique ? | Nb de pays uniques / indice de diversité | Évaluer la stratégie de globalisation |

---

## 🧠 Mon rôle à cette étape

- Comprendre les **besoins métiers** avant toute manipulation de données.  
- Traduire ces besoins en **KPI mesurables** et pertinents.  
- Identifier les **colonnes du dataset** nécessaires à chaque KPI.  
- Préparer la feuille de route analytique pour les étapes suivantes.

---

## 🧩 Correspondance KPI ↔ Variables du dataset

| KPI | Variables du dataset Kaggle |
|------|-----------------------------|
| % Films / Séries | `type` |
| Nb de titres par pays | `country` |
| Genres dominants | `listed_in` |
| Croissance annuelle | `date_added`, `release_year` |
| Répartition par rating | `rating` |
| Diversité géographique | `country`, `year_added` |


📁 **Étape suivante :** [Préparation et nettoyage des données →](./netflix_data_analysis.md)
