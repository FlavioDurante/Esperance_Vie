# Prédiction de l'Espérance de Vie

Dans ce projet de machine learning, nous analysons les données de santé et économiques de 193 pays (2000-2015) issues de l’OMS et de l’ONU 

Après un nettoyage des données, nous effectuons une analyse exploratoire pour identifier les facteurs critiques influençant l’espérance de vie. 

Enfin, nous développons un modèle prédictif basé sur ces variables pour estimer l’espérance de vie en fonction des indicateurs de santé et économiques.

## Table des matières
1. [Présentation](#présentation)
2. [Données](#données)
3. [Structure du projet](#structure-du-projet)
4. [Installation & Usage](#installation--usage)
5. [Modèles entraînés](#modèles-entraînés)
6. [Résultats](#résultats)
7. [Licence](#licence)

## Données
- **Source** : OMS et de l’ONU, accessible via ce lien https://www.kaggle.com/code/varunsaikanuri/life-expectancy-visualization/input

| Nom de la variable                       | Type de donnée | Unité / Mesure          | Description                                                                                      |
|------------------------------------------|----------------|-------------------------|--------------------------------------------------------------------------------------------------|
| `Country`                                | Qualitatif     | —                       | Pays concerné                                                                                     |
| `Year`                                   | Quantitatif    | Année (YYYY)            | Année de l’observation                                                                           |
| `Status`                                 | Qualitatif     | —                       | Catégorie de développement (« Developing », « Developed »)                                        |
| `Life expectancy`                        | Quantitatif    | Années                  | Espérance de vie à la naissance                                                                   |
| `Adult Mortality`                        | Quantitatif    | Taux pour 1000 adultes  | Mortalité adulte (15–60 ans)                                                                      |
| `infant deaths`                          | Quantitatif    | Nombre d’enfants        | Nombre de décès d’enfants de moins d’un an                                                        |
| `Alcohol`                                | Quantitatif    | Litres par personne     | Consommation annuelle d’alcool par habitant                                                      |
| `percentage expenditure`                 | Quantitatif    | % du PIB                | Dépenses de santé totales en pourcentage du PIB                                                  |
| `Hepatitis B`                            | Quantitatif    | % de couverture         | Taux de couverture vaccinale contre l’hépatite B chez les enfants                                 |
| `Measles`                                | Quantitatif    | Cas pour 1000 enfants   | Nombre de cas de rougeole signalés (taux pour 1000 enfants de moins de 5 ans)                    |
| `BMI`                                    | Quantitatif    | kg/m²                   | Indice de masse corporelle moyen de la population                                                 |
| `under-five deaths`                      | Quantitatif    | Nombre d’enfants        | Nombre de décès d’enfants de moins de 5 ans                                                       |
| `Polio`                                  | Quantitatif    | % de couverture         | Taux de couverture vaccinale contre la poliomyélite chez les enfants                              |
| `Total expenditure`                      | Quantitatif    | % du PIB                | Dépenses totales de santé en pourcentage du PIB (note : parfois redondant avec « percentage expenditure 
| `Diphtheria`                             | Quantitatif    | % de couverture         | Taux de couverture vaccinale contre la diphtérie                                                  |
| `HIV/AIDS`                               | Quantitatif    | Taux pour 1000 personnes| Prévalence ou taux de mortalité dû au VIH/SIDA (/1000 hab.)                                       |
| `GDP`                                    | Quantitatif    | USD par habitant        | Produit intérieur brut par habitant                                                              |
| `Population`                             | Quantitatif    | Nombre d’habitants      | Population totale                                                                                 |
| `thinness 1-19 years`                    | Quantitatif    | % de prévalence         | Prévalence du thinness (émaciation) chez les 10–19 ans                                            |
| `thinness 5-9 years`                     | Quantitatif    | % de prévalence         | Prévalence du thinness (émaciation) chez les 5–9 ans                                             |
| `Income composition of resources`        | Quantitatif    | Indice (0–1)            | Indice de composition des ressources de revenu (mesure d’inégalité)                                |
| `Schooling`                              | Quantitatif    | Années                  | Nombre moyen d’années de scolarisation                                                          |

## Structure du projet
├── Life.ipynb # EDA & Models

├── Life Expectancy Data.csv # Données

## Installation & Usage
```bash
git clone https://…/Esperance_Vie.git

```
## Modèles entraînés
XGBoost

Ridge

## Enjeux & résultats
XGBoost:
----------------------------


R2 su train:  0.997716535183886

R2 su validazione:  0.9477611954988485

MSE su train:  0.2059863733046369

MSE su validazione:  4.760513726614255

Average expected loss (MSE): 5.716

Average bias: 4.923

Average variance: 0.792


Ridge:
--------------------------


R2 su train:  0.8466435314381352

R2 su validazione:  0.8340007664358708

MSE su train:  13.83395205345207

MSE su validazione:  15.12748305662438

## Licence
Ce projet est sous licence MIT.
