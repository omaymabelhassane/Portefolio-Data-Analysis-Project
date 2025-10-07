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

## 🧭 Cheminement analytique

### 1) Préparation & features
- Normaliser `date_added` → colonnes **année**, **mois**.  
- Uniformiser `duration` (minutes pour films / saisons pour séries).  
- Nettoyer `listed_in` (genres) & exploser les **pays** si analyse fine.  
- Gérer **NA/doublons** (règles documentées).

### 2) Analyse descriptive (EDA)
- **Évolution** du catalogue par année (Movie vs TV Show).  
- **Répartition géographique** et top pays producteurs.  
- **Genres** dominants (Top 10) et évolution.  
- **Ratings** (classification d’âge) et tendances.  
- **Durée** moyenne par type/genre.

### 3) Modèle BI & Dashboard
- **Dimensions :** Temps, Pays, Genre, Type, Rating.  
- **Mesures (exemples) :** `#Titres`, `%Séries`, `#Pays`,
