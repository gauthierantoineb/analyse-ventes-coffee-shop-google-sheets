# Analyse des ventes d’un coffee shop

Projet de **Sales Analytics / Business Intelligence** réalisé dans **Google Sheets** à partir de données transactionnelles d’un coffee shop.  
L’objectif du projet est d’identifier les principaux leviers de performance commerciale à travers l’analyse des produits, des horaires de vente et des dynamiques temporelles, puis de formuler des recommandations opérationnelles.

---

## Vue d’ensemble

Ce projet porte sur l’analyse des transactions d’un coffee shop entre **mars 2024 et mars 2025**.  
À partir d’un dataset transactionnel, j’ai construit une analyse orientée décision pour répondre à une question business simple :

> **Quels sont les principaux drivers du chiffre d’affaires du coffee shop, et quels leviers d’action peuvent être activés pour améliorer la performance ?**

L’analyse a été réalisée dans **Google Sheets** à l’aide de :
- colonnes dérivées
- tableaux croisés dynamiques
- graphiques
- synthèse business finale

---

## Résumé exécutif

L’analyse met en évidence trois enseignements principaux :

- **Le chiffre d’affaires est fortement concentré sur quelques références clés** : Latte, Americano with Milk et Cappuccino représentent à eux trois **61,5 % du chiffre d’affaires total**.
- **La performance varie fortement selon le temps** : **10h** est l’heure la plus contributive en chiffre d’affaires, et les jours de semaine performent mieux que le week-end.
- **Les recommandations prioritaires** portent sur le staffing des créneaux les plus forts, la mise en avant des produits les plus contributifs et l’animation commerciale des périodes les plus faibles.

---

## Contexte business

Le management d’un coffee shop dispose de données de ventes, mais n’a pas forcément une vision claire de :
- ce qui génère réellement le chiffre d’affaires
- quels produits contribuent le plus à la performance
- quels moments de la journée ou de la semaine concentrent l’activité
- où concentrer les efforts opérationnels et commerciaux

Ce projet vise donc à transformer des données transactionnelles brutes en **insights actionnables**.

---

## Décision business à éclairer

Cette analyse vise à aider à prioriser les décisions suivantes :

- quels produits mettre davantage en avant
- quels créneaux nécessitent le plus d’attention opérationnelle
- quels moments plus faibles pourraient être stimulés par des actions commerciales ciblées

---

## Dataset

Le dataset contient des transactions de vente avec notamment :
- la date de transaction
- l’heure de transaction
- le nom du produit
- le mode de paiement
- le montant de la transaction

### Grain analytique
Le **grain principal d’analyse** est la **transaction de vente**.

### Population analysée
L’analyse porte sur **3 547 transactions**.

### Période étudiée
**Mars 2024 à mars 2025**, avec prudence sur **mars 2024** et **mars 2025**, qui sont des mois partiels.

### Variables dérivées créées pendant l’analyse

Pour enrichir l’analyse, plusieurs dimensions ont été construites dans Google Sheets :

- `annee`
- `annee_mois`
- `nom_mois`
- `jour_semaine`
- `ordre_jour_semaine`
- `est_weekend`
- `heure_achat`
- `moment_journee`
- `ordre_moment_journee`

### Source du dataset
Dataset public Kaggle :  
[Coffee Revenue Dataset](https://www.kaggle.com/datasets/rifatalam3/coffee-revenue-dataset?resource=download)

---

## Outils utilisés

- **Google Sheets**
- **Colonnes calculées**
- **Tableaux croisés dynamiques**
- **Graphiques**
- **Synthèse business / reporting**

---

## Objectif analytique

L’analyse vise à répondre à trois questions principales :

1. **Quels produits contribuent le plus au chiffre d’affaires ?**
2. **Quels moments de la journée et quels jours performent le mieux ?**
3. **Quels leviers business semblent les plus pertinents pour améliorer la performance ?**

---

## Démarche analytique

### 1. Nettoyage et préparation des données
- standardisation des dates et des heures
- renommage des colonnes
- création de dimensions analytiques
- vérification de la cohérence des données

### 2. Construction des KPI
KPI principaux construits dans le projet :
- nombre de transactions
- chiffre d’affaires total
- ticket moyen
- chiffre d’affaires moyen par jour

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
- formulation d’insights clés
- recommandations opérationnelles
- explicitation des limites de l’analyse

---

## KPI principaux

- **Nombre de transactions** : 3 547
- **Chiffre d’affaires total** : 112 245,58
- **Ticket moyen** : 31,64
- **CA moyen par jour** : 294,61

---

## Insights clés

### 1. Forte concentration du chiffre d’affaires
**Latte, Americano with Milk et Cappuccino génèrent 61,5 % du chiffre d’affaires total.**  
La performance commerciale repose donc fortement sur un nombre limité de produits.

### 2. Le produit le plus vendu n’est pas le plus contributif en valeur
**Americano with Milk** est le produit le plus vendu avec **809 transactions**, tandis que **Latte** génère le plus de chiffre d’affaires avec **26 875,30**.  
Cela montre qu’il est important de distinguer **volume** et **valeur** dans l’analyse.

### 3. La temporalité influence fortement la performance
**10h** est l’heure la plus contributive en chiffre d’affaires avec **10 198,52**.  
À l’échelle des grands moments de la journée, **le soir** ressort légèrement devant en chiffre d’affaires total.

### 4. Les jours de semaine performent mieux que le week-end
Le chiffre d’affaires journalier moyen est plus élevé en semaine qu’en week-end :

- **Semaine** : 309,47
- **Week-end** : 257,52

Soit un écart d’environ **+20,2 %** en faveur des jours de semaine.

---

## Recommandations business

### 1. Renforcer l’organisation sur les créneaux les plus porteurs
Les créneaux de forte activité, notamment autour de **10h** et sur certaines plages de l’après-midi et du soir, doivent être priorisés en matière de :
- staffing
- préparation
- gestion du flux

### 2. Capitaliser sur les produits les plus contributifs
**Latte, Cappuccino et Americano with Milk** devraient bénéficier d’une mise en avant renforcée via :
- la signalétique
- les suggestions de vente
- des offres combinées
- des bundles

### 3. Stimuler les périodes les moins dynamiques
Les périodes les moins performantes, notamment certains créneaux du week-end, peuvent faire l’objet d’actions ciblées :
- promotions ponctuelles
- bundles
- animation commerciale
- offres limitées dans le temps

---

## Limites de l’analyse

Cette analyse présente plusieurs limites importantes :

- un seul mode de paiement est disponible, ce qui empêche toute comparaison selon le moyen de paiement
- aucun identifiant client n’est disponible, donc il n’est pas possible d’analyser la fidélité, la rétention ou le repeat purchase
- le dataset ne contient ni coût, ni marge, ni source d’acquisition
- mars 2024 et mars 2025 sont des mois partiels, donc leur comparaison avec des mois complets doit être interprétée avec prudence

En conséquence, ce projet doit être lu comme une **analyse descriptive transactionnelle orientée décision**, et non comme une analyse client ou une analyse de rentabilité complète.

---

## Compétences démontrées

- nettoyage et préparation de données transactionnelles
- création de variables dérivées dans Google Sheets
- construction de KPI business
- analyse produit
- analyse temporelle
- création de tableaux croisés dynamiques
- data storytelling
- formulation de recommandations opérationnelles
- explicitation des limites analytiques

---

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
