---
title: "Series.PointValues"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Series. Obtient les valeurs réelles utilisées pour tracer chaque point de cette série dans le graphique"
type: docs
url: /fr/net/aspose.cells.charts/series/pointvalues/
---
## Series.PointValues property

Obtient les valeurs réelles utilisées pour tracer chaque point de cette série dans le graphique.

```csharp
public ChartDataValue[] PointValues { get; }
```

### Remarques

Cette propriété offre un moyen pratique d'obtenir les valeurs réelles correspondant aux données définies par [`Values`](../values/), en particulier lorsque la source de données spécifiée est un lien externe, une formule, ...etc.

### Exemples

```csharp
//Démo montrant un cas qui nécessite cette propriété :
[C#]

Workbook workbook = new Workbook("ExternalSourceChart.xlsx");
Worksheet worksheet = workbook.Worksheets[0];
Chart chart = worksheet.Charts[0];
chart.Calculate();
string Values = chart.NSeries[0].Values;
// Les valeurs pourraient être comme "[External.xlsx]Sheet1!$A$1:$A$6" ce qui est compliqué
// pour que l'utilisateur obtienne les valeurs réelles (les valeurs peuvent être liées à un autre classeur,
// ou mises en cache dans le classeur actuel). Ici vous pouvez utiliser la propriété PointValues
// pour obtenir les valeurs réellement affichées dans l'interface Excel
// sous forme de tableau.
ChartDataValue[] v1 = chart.NSeries[0].PointValues;

```

### Voir aussi

* class [ChartDataValue](../../chartdatavalue/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


