# Analyse des ventes d’un coffee shop

Projet de **Sales Analytics / Business Intelligence** réalisé dans **Google Sheets** à partir de données transactionnelles d’un coffee shop, avec nettoyage des données, création de KPI, analyses produit et temporelles, puis recommandations opérationnelles.

## Vue d’ensemble du projet

Ce projet analyse les transactions d’un coffee shop entre **mars 2024 et mars 2025**.  
L’objectif est d’identifier les principaux moteurs du chiffre d’affaires à travers :

- l’analyse des produits
- l’analyse des heures de vente
- l’analyse des jours de semaine
- l’analyse des tendances mensuelles
- la formulation de recommandations business

L’analyse a été réalisée dans **Google Sheets** à l’aide de colonnes dérivées, tableaux croisés dynamiques, graphiques et d’une synthèse finale.

---

## Objectif business

L’objectif principal du projet est de répondre à la question suivante :

**Quels sont les principaux drivers du chiffre d’affaires du coffee shop, et quels leviers d’action peuvent être activés pour améliorer la performance ?**

---

## Dataset

Le dataset contient des transactions de ventes avec des informations comme :

- la date de transaction
- l’heure de transaction
- le nom du produit
- le mode de paiement
- le montant de la transaction

### Variables dérivées créées pendant l’analyse

- `annee`
- `annee_mois`
- `nom_mois`
- `jour_semaine`
- `ordre_jour_semaine`
- `est_weekend`
- `heure_achat`
- `moment_journee`
- `ordre_moment_journee`

source d’origine du dataset : https://www.kaggle.com/datasets/rifatalam3/coffee-revenue-dataset?resource=download

---

## Outils utilisés

- **Google Sheets**
- Tableaux croisés dynamiques
- Colonnes calculées
- Graphiques
- Reporting business

---

## Démarche analytique

### 1. Nettoyage et préparation des données
- standardisation des dates et des heures
- renommage des colonnes
- création de dimensions analytiques
- vérification de la cohérence des données

### 2. Construction des KPI
KPI principaux construits dans le projet :
- Nombre de transactions
- Chiffre d’affaires total
- Ticket moyen
- Chiffre d’affaires moyen par jour

### 3. Analyse produit
- chiffre d’affaires par produit
- nombre de transactions par produit
- ticket moyen par produit

### 4. Analyse temporelle
- chiffre d’affaires par heure
- nombre de transactions par heure
- ticket moyen par heure
- chiffre d’affaires par moment de la journée
- chiffre d’affaires par jour de semaine
- évolution mensuelle du chiffre d’affaires

### 5. Synthèse business
- insights clés
- recommandations opérationnelles
- limites de l’analyse

---

## KPI principaux

- **Nombre de transactions :** 3 547
- **Chiffre d’affaires total :** 112 245,58
- **Ticket moyen :** 31,64
- **CA moyen par jour :** 294,61

---

## Insights clés

### 1. Concentration du revenu
Latte, Americano with Milk et Cappuccino génèrent **61,5 % du chiffre d’affaires total**, ce qui montre une forte concentration du revenu sur trois références clés.

### 2. Volume vs valeur
Americano with Milk est le **produit le plus vendu (809 transactions)**, tandis que Latte génère le **plus de chiffre d’affaires (26 875,30)**. Cela suggère un meilleur équilibre entre volume vendu et valeur unitaire pour Latte.

### 3. Temporalité des ventes
**10h** est l’heure la plus contributive en chiffre d’affaires (**10 198,52**). À l’échelle des grands moments de la journée, le **soir** est légèrement devant en chiffre d’affaires total.

### 4. Semaine vs week-end
Le chiffre d’affaires journalier moyen est plus élevé en semaine qu’en week-end :
- **Semaine :** 309,47
- **Week-end :** 257,52

Soit un écart d’environ **+20,2 %** en faveur des jours de semaine.

---

## Recommandations business

### 1. Renforcer l’organisation sur les créneaux les plus porteurs
Les créneaux de forte activité, notamment autour de **10h** et sur certaines plages de l’après-midi et du soir, doivent être priorisés en matière de staffing, préparation et gestion du flux.

### 2. Capitaliser sur les produits les plus contributifs
Latte, Cappuccino et Americano with Milk devraient bénéficier d’une mise en avant renforcée via la signalétique, les suggestions de vente et des offres combinées.

### 3. Stimuler les périodes les moins dynamiques
Les périodes les moins performantes, notamment certains créneaux du week-end, peuvent faire l’objet d’actions ciblées : promotions ponctuelles, bundles ou animations commerciales.

---

## Limites de l’analyse

Cette analyse présente plusieurs limites :

- un seul mode de paiement est disponible, ce qui empêche toute comparaison des comportements selon le moyen de paiement
- aucun identifiant client n’est disponible, donc il n’est pas possible d’analyser la fidélité, la rétention ou le repeat purchase
- le dataset ne contient ni coût, ni marge, ni source d’acquisition
- mars 2024 et mars 2025 sont des mois partiels, donc leur comparaison avec des mois complets doit être interprétée avec prudence

---

## Compétences démontrées

- Nettoyage et préparation de données transactionnelles
- Création de variables dérivées dans Google Sheets
- Construction de KPI business
- Analyse produit et analyse temporelle
- Création de tableaux croisés dynamiques
- Data storytelling et recommandations opérationnelles

## Structure du dépôt

```text
analyse-ventes-coffee-shop-google-sheets/
│
├── README.md
├── donnees/
│   └── Coffe_sales (1).xlsx
├── captures/
│   ├── 1_donnees_brutes.png
│   ├── 2_donnees_nettoyees.png
│   ├── 3_kpi.png
│   ├── 4_analyse_produit.png
│   ├── 5_analyse_temporelle.png
│   └── 6_rapport.png
└── livrables/
    └── rapport_ventes_coffee_shop.pdf
