# 📊 Analyse de Données — E-commerce Price Intelligence Platform

> **Projet :**  Real-Time E-commerce Price Intelligence Platform
> 
> **Couche :** Analysis Layer
> 
> **Auteure :** Basma ABIS 


## 📁 Structure du projet

```
data-analysis/
├── notebooks/
│   ├── Data_Exploration.ipynb           # Chargement, audit qualité, nettoyage
│   ├── Descriptive_Statistics.ipynb     # Stats descriptives, visualisations, tendances
│   └── Inferential_Statistics.ipynb     # Tests statistiques, régression, power analysis
├── outputs/
│   ├── descriptive_statistics/
│   │   ├── tables/                      # Tableaux CSV (moyenne, écart-type, volatilité)
│   │   └── figures/                     # Graphiques PNG (boxplots, histogrammes, séries temporelles)
│   └── inferential_statistics/
│       ├── tables/                      # Résultats des tests (Mann-Whitney, ANOVA, régression)
│       ├── figures/                     # Q-Q plots, résidus, courbe de puissance
│       └── reports/                     # Interprétations business
├── data/processed/                      # Dataset nettoyé au format Parquet                   
├── docker-compose.yml
├── requirements.txt
└── .gitignore
```

---

##  Analyses réalisées

###  Statistiques descriptives

| Analyse | Résultat produit |
|
| Moyenne et médiane des prix | Par plateforme et global |
| Volatilité des prix | Écart-type + coefficient de variation |
| Distribution des remises | Montant et pourcentage de réduction |
| Tendances par catégorie/marque | Top 10 marques |
| Évolution des prix dans le temps | Série temporelle par date de collecte |

###  Statistiques inférentielles

| Test | Objectif |
|
| Shapiro-Wilk | Vérification de la normalité |
| Mann-Whitney U | Comparaison des prix entre deux plateformes |
| Kruskal-Wallis / ANOVA | Comparaison sur les trois plateformes |
| Régression OLS | Prix ~ note + avis + temps + plateforme |
| Intervalles de confiance (95%) | Estimation du prix moyen par plateforme |
| Power Analysis | Vérification de la taille d'échantillon |



*Basma ABIS — Data Analyst · E-commerce Price Intelligence · *
