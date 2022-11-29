# 1. Data Ingestion & Transformation (hint)
- rawData est obtenue à partir d'un simple copier-coller d'un tableau excel :
```
rawData = 'données\tBrutes'
```
- Séparation des données par tabulation '\t' 
- D3 dispose d'un nombre de fonctions pour appliquer les transformations initiales aux données
- extension .tsv = tab separated values / extension .csv = comma separated values
```
tsvData = d3.tsvParse(rawData)
```
- Estimation automatique des types de données :
```
tsvAutoTypedData = d3.tsvParse(rawData, d3.autoType)
```
- Définition manuelle des types de données :
```
tsvExplicitTypedData = d3.tsvParse(rawData,({ Entity, Year, Actual_Estimate, Projection }) => ({
    Entity: Entity,
    Year: d3.timeParse("%Y")(Year),
    Actual_Estimate: +Actual_Estmiate,
    Projection: +Projection,
    Summary: +Actual_Estimate + +Projection
})
```
- La data à utiliser pour la visualisation
```
useData = tsvExplicitTypedData
```
- Regroupement des données par Entité:
```
groupedData = d3.group(tsvExplicitTypedData, (d) => d["Entity"])
```
