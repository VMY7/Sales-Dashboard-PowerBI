# Sales-Dashboard-PowerBI
## 🎯 Objectif
Créer un dashboard interactif qui permet de suivre la performance commerciale d’une entreprise fictive : évolution des ventes, top produits, analyse régionale et performance des vendeurs.

---

## 📂 Étapes du projet
### 1. Création du dataset (Excel/CSV)
- Colonnes principales :
  - Date (sur 1 an, ex. 2024 complet)
  - Produit (10–15 produits simulés)
  - Catégorie (ex. Électronique, Maison, Vêtements, Alimentation…)
  - Région (ex. Nord, Sud, Est, Ouest)
  - Vendeur (5–6 commerciaux)
  - Quantité (nombre d’articles vendus)
  - PrixUnitaire
  - Ventes (Quantité × PrixUnitaire)
  - Coût (Quantité × PrixCoût)
  - Marge (Ventes – Coût)

---

### 2. Préparation dans Power Query
- Vérifier les types de données (date, numérique, texte).
- Ajouter colonnes dérivées si besoin (ex. Année, Mois, Marge%).

---

### 3. KPI & mesures DAX
- `Total Ventes = SUM(Ventes)`
- `Total Quantité = SUM(Quantité)`
- `Marge Totale = SUM(Marge)`
- `Marge % = DIVIDE(SUM(Marge), SUM(Ventes))`
- `Ventes Mois N-1, Croissance MoM (mesures temporelles).`
---

### 4. Dashboard Power BI
- Vue globale :
  - Carte KPI (ventes totales, marge, quantité).
  - Line chart → évolution des ventes par mois.
- Analyse produits :
  - Bar chart top 10 produits.
  - Répartition des ventes par catégorie (camembert ou donut).
- Analyse géographique :
  - Carte ou bar chart par région.
- Performance vendeurs :
  - Classement des commerciaux (ventes & marge).

---

### 5. Storytelling métier
- Répondre à des questions type :
  - Quel produit rapporte le plus ?
  - Quelle région est la plus performante ?
  - Quel vendeur surperforme ?
  - Quelle tendance mensuelle se dégage ?
