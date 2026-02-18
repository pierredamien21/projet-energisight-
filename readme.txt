# GreenSight Lomé : Intelligence Artificielle et Résilience Énergétique

## Description du Projet
**GreenSight** (également désigné sous le nom d'**EnergiSight**) est une initiative technologique d'avant-garde visant à modéliser la consommation énergétique et l'empreinte carbone du parc immobilier non résidentiel de la ville de Lomé, au Togo. 

Face à une asymétrie d'information notoire et à l'absence de cadastres énergétiques numérisés, ce projet utilise le **Transfer Learning** (Apprentissage par Transfert) pour transposer les lois physiques apprises sur des métropoles riches en données (Seattle) vers les réalités sociomorphologiques togolaises.

---

## Contexte et Problématique
L'urbanisation galopante de Lomé impose une pression croissante sur le réseau de la **CEET**. Cependant, la planification urbaine est entravée par :
- **Le Silence des Données** : Manque de compteurs intelligents et de données historiques granulaires.
- **La Complexité Logistique** : Coût prohibitif des relevés physiques manuels.
- **Le Défi Climatique** : Nécessité d'identifier les bâtiments énergivores pour orienter les politiques de rénovation.

GreenSight apporte une réponse à cette problématique en transformant la donnée géographique brute en intelligence énergétique.

---

## Spécifications Techniques

### Méthodologie : Le Paradigme du Transfer Learning
Le cœur de la solution repose sur l'algorithme **XGBoost (Extreme Gradient Boosting)**. Le processus se décline en trois étapes majeures :
1. **Apprentissage Source** : Capture des corrélations universelles (Surface/Consommation) sur le dataset de Seattle.
2. **Fine-Tuning** : Ajustement des poids statistiques aux réalités de Lomé.
3. **Calibration Locale** : Intégration des données du **RGPH 2022** pour refléter la diversité du bâti (Banco, Semi-moderne, Moderne).

### Ingénierie des Caractéristiques (Feature Engineering)
- **Transformation Logarithmique** : Appliquée aux cibles pour stabiliser la variance et gérer les valeurs extrêmes (outliers).
- **Normalisation Z-score** : Standardisation des variables numériques pour une contribution équitable au modèle.
- **Encodage Categoriel** : Traitement par *One-Hot Encoding* des types d'usages et de la qualité constructive.



### Arsenal Technologique
- **Langage** : Python 3.12
- **Analyse** : Pandas, NumPy, Scipy
- **Machine Learning** : Scikit-Learn, XGBoost
- **Visualisation** : Matplotlib, Seaborn
- **Interface** : Streamlit (en cours de déploiement)

---

## Résultats et Performances
Les modèles actuels affichent des métriques de haute fiabilité :
- **Modèle CO2** : Coefficient de détermination $R^2 = 0.91$.
- **Modèle Énergie** : Coefficient de détermination $R^2 = 0.84$.
- **Validation sur Lomé** : Précision de 99% sur le dataset de calibration locale grâce à l'intégration des variables de qualité du bâti.

---
