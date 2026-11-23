---
title: "GridPivotTable.CalculateData"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "GridPivotTable méthode. Calcule les données des tableaux croisés dynamiques vers les cellules"
type: docs
url: /fr/net/aspose.cells.gridweb.data/gridpivottable/calculatedata/
---
## GridPivotTable.CalculateData method

Calcule les données du pivottable vers les cellules.

```csharp
public void CalculateData()
```

### Remarques

Cell.Value dans la plage pivot ne peut pas renvoyer le résultat correct si la méthode n'a pas été appelée. Cette méthode calcule les données avec un cache pivot interne, pas la source de données originale. Ainsi, si la source de données est modifiée, veuillez appeler la méthode RefreshData() en premier.

### Voir aussi

* class [GridPivotTable](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


