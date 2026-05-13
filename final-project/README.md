# Ienākumu prognozēšana — izglītība un dzimums ASV datos

## Problēma
Prognozēt vai ASV iedzīvotāja ienākumi pārsniedz 
$50,000 gadā. Pētām izglītības un dzimuma ietekmi 
uz ienākumu līmeni.

## Datasets
- Avots: https://www.kaggle.com/datasets/uciml/adult-census-income
- Izmērs: 32,561 rindas × 15 kolonnas
- Target kolonna: income (<=50K vai >50K)

## Pieeja
- ML tips: Klasifikācija
- Pipeline: OneHotEncoder + StandardScaler → LogisticRegression
- Optimizācija: GridSearchCV (C, solver)

## Rezultāti
- Bāzes modelis: CV F1 = 0.604 ± 0.067
- Labākais modelis: Logistic Regression CV F1 = 0.602
- Galvenās pazīmes: capital.gain, sex_Female, education.num

## Kā palaist
1. `pip install -r requirements.txt`
2. Atver `notebooks/final_project.ipynb`
3. Izpildi visas šūnas (Kernel → Restart & Run All)

## Autors
Eva, FITA ML kurss, 2026
