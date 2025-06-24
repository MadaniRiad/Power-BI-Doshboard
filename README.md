# Power-BI-Dashboard – Analyse du Churn Client pour ABC Bank

📊 **Tableaux de bord interactifs Power BI** pour analyser et anticiper le départ des clients (churn) d'**ABC Bank**, une banque multinationale. Ce projet s'inscrit dans une démarche décisionnelle visant à identifier les profils les plus susceptibles de quitter la banque et proposer des actions de fidélisation.

---

## 🎯 Objectifs du projet

- Étudier le phénomène de **churn client** (taux d'attrition) via une analyse de données.
- Identifier les **profils à risque** de départ (âge, genre, activité, région, score client…).
- Aider les équipes métier (**CRM, marketing, direction commerciale**) à prendre des **décisions stratégiques**.

---

## 👥 Équipe projet

- **Professeur encadrant** : Eliana  
- **Réalisé par** :
  - Abdelkrim  
  - Riad

---

## 🧑‍💼 Clients finaux

- Directeur Marketing
- Responsable CRM
- Équipe commerciale

---

## 🔍 Problématique

Le **churn** représente un enjeu stratégique : fidéliser un client coûte **moins cher** qu’en acquérir un nouveau. Ce projet vise à créer un outil visuel (dashboard Power BI) permettant :

- d'**anticiper les départs clients**
- d’**identifier les causes du churn**
- de **segmenter la clientèle à risque**
- et de **suivre les indicateurs de fidélisation**

---

## 🧰 Données utilisées

Les données proviennent d’un entrepôt de données simulé, réparties sur plusieurs fichiers CSV, incluant :

- Données clients : âge, genre, solde, salaire, score, nombre d’années client…
- Données comportementales : activité, port de carte, churn (oui/non)
- Données géographiques
- Données temporelles

### 🔗 Modélisation en étoile

La structure du modèle repose sur une **table de faits `BANK_CHURN`** reliée à plusieurs **dimensions** :

- `CUSTOMER_INFO`
- `EXIT_CUSTOMER`
- `ACTIVE_CUSTOMER`
- `CREDIT_CARD`
- `GEOGRAPHI`
- `DATE`
- `GENDER`

---

## 🔨 Préparation & Transformation des données

Effectuée via **Power Query** dans Power BI :

- Conversion de types (ex : CustomerID → texte)
- Suppression des colonnes inutiles et valeurs nulles
- Création de colonnes dérivées :
  - `Score_type` (Médiocre → Excellent)
  - `Catégorie_age` (Adolescent, Jeune, Adulte, Aîné)
  - Colonnes temporelles : `Année`, `Mois`, `Trimestre`, `YearMonth`, etc.
- Renommage pour clarification

---

## 📊 Visualisations proposées

Les dashboards construits dans Power BI permettent une **analyse multidimensionnelle** du churn :

### ✅ Indicateurs clés

- Taux d’attrition (churn)
- Taux de fidélisation
- Nombre total de clients
- Répartition actif / inactif
- Solde et salaire moyen
- Nombre moyen d’années de fidélité

### 📈 Types de visualisations utilisées

| Type            | Utilisation principale                                              |
|-----------------|---------------------------------------------------------------------|
| Line Chart      | Évolution du churn par région ou par profil                         |
| Bar Chart       | Comparaison actif/inactif, churn/fidélisé                          |
| Carte géographique | Répartition régionale du churn                                     |
| Camembert       | Répartition des churners par genre                                  |
| Sparklines      | Suivi des tendances par mois ou année                               |

---

## ❓ Requêtes d’analyse posées

- Quels profils sont les plus susceptibles de quitter la banque ?
- Le churn est-il plus fort chez les jeunes, les femmes, les inactifs ?
- Quelle région enregistre le taux de churn le plus élevé ?
- Y a-t-il une corrélation entre score bancaire et churn ?
- Évolution du churn sur les 2 dernières années ?

---

## 🧠 Insights & Conclusions

- **Les jeunes clients féminins inactifs** sont les plus susceptibles de quitter.
- Le **score client initial** est fortement corrélé au départ futur.
- La **région allemande** montre un taux de churn très préoccupant.
- Une **campagne de fidélisation ciblée** est indispensable.

---

## 🧩 Recommandations

- Lancer des **campagnes marketing ciblées** (femmes, jeunes)
- Revoir les **processus d'onboarding** pour améliorer l’engagement
- Développer des **programmes de fidélité**
- Suivre en continu les **KPIs de churn** pour réagir rapidement

---

## 📎 Dossier de projet

- 📁 `./datasets/` — Données CSV utilisées pour l’analyse
- 📁 `./reports/` — Rapport complet du projet
- 📄 `Dashboard.pbix` — Fichier Power BI contenant les visualisations

---

## 💡 À propos

Projet réalisé dans le cadre du module **Entrepôt de Données**, avec un focus sur la **modélisation décisionnelle** et la **dataviz métier**.

---

## 📜 Licence

Projet académique — aucune licence commerciale.
