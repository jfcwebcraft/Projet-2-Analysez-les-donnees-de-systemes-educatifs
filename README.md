# Projet 2 · Analysez les données de systèmes éducatifs

**Parcours Data Engineer & IA — OpenClassrooms**  
**Entreprise cliente :** Academy (start-up EdTech)  
**Auteur :** Jean-François Chaussoy  
**Date :** Décembre 2025 – Janvier 2026  

---

## 🎯 Contexte et problématique métier

La start-up EdTech **Academy**, spécialisée dans les formations en ligne sur les technologies d'avenir, souhaite développer son activité à l'international. 

L'objectif de cette mission est de réaliser une **analyse exploratoire approfondie** des données éducatives mondiales fournies par la Banque Mondiale (**EdStats**), afin d'éclairer la stratégie d'expansion géographique de l'entreprise.

### Questions clés traitées :
1. Quels pays présentent un potentiel élevé d'expansion pour les services éducatifs d'Academy ?
2. Pour chacun de ces pays, quelle sera l'évolution prévisible de la population étudiante ?
3. Vers quels pays cibler prioritairement les investissements marketing ?

---

## 📊 Méthodologie & Réalisations

1. **Nettoyage et validation des données (Data Cleaning) :**
   - Exploration du jeu de données EdStats (plus de 4 000 indicateurs internationaux).
   - Traitement des valeurs manquantes, détection des valeurs aberrantes et sélection des indicateurs les plus pertinents et fiables.
2. **Analyse exploratoire des données (EDA) :**
   - Statistiques descriptives univariées et bivariées (distribution, dispersion, corrélations).
   - Analyse démographique (projection des tranches d'âge 15-24 ans).
   - Analyse des infrastructures numériques (taux d'équipement, pénétration d'Internet).
3. **Score d'opportunité multicritères (Scoring EdTech) :**
   - Modélisation d'un score composite combinant potentiel démographique, niveau d'éducation tertiaire et maturité numérique.
   - Classement des pays cibles avec restitution visuelle et analyse de sensibilité.

---

## 📂 Organisation du dépôt

```text
├── Academy Exercice 1/
│   ├── Projet_2_Analysez_les_données_de_systèmes_éducatifs_.ipynb  # Notebook Jupyter complet
│   ├── pyproject.toml                                            # Dépendances du projet
│   ├── EdStatsCountry.csv                                        # Métadonnées pays
│   ├── EdStatsSeries.csv                                         # Métadonnées séries
│   └── EdStatsCountry-Series.csv                                 # Relations pays-séries
├── Support de présentation Projet 2.pdf                          # Support de soutenance (30 slides)
├── P2+_+Data+Engineer-+Fiche+d_auto-évaluation.pdf               # Grille d'auto-évaluation
├── resultats_scoring_edtech_FR.csv                               # Résultats du scoring final
├── .gitignore
└── README.md
```

> **Note sur le jeu de données volumineux :**  
> Le fichier brut `EdStatsData.csv` (> 320 Mo) est exclu du dépôt Git conformément aux bonnes pratiques. Il peut être téléchargé directement depuis la plateforme [World Bank EdStats](https://databank.worldbank.org/source/education-statistics-%7e-all-indicators).

---

## 🛠️ Stack technique

* **Python 3.10+**
* **Pandas & NumPy** : Manipulation, agrégation et nettoyage de données volumineuses.
* **Matplotlib & Seaborn** : Visualisations statistiques et graphiques exploratoires.
* **Jupyter Notebook** : Analyse reproductible et documentée.
