---
title: "Series.CategoryValues"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Series. Obtient les valeurs de catégorie réelles utilisées pour tracer chaque point de cette série dans le graphique"
type: docs
url: /fr/net/aspose.cells.charts/series/categoryvalues/
---
## Series.CategoryValues property

Obtient les valeurs de catégorie réelles utilisées pour tracer chaque point de cette série dans le graphique.

```csharp
public ChartDataValue[][] CategoryValues { get; }
```

### Remarques

Cette propriété offre un moyen pratique d'obtenir les valeurs réelles correspondant aux données définies par [`XValues`](../xvalues/), en particulier lorsque la source de données spécifiée est un lien externe, une formule, etc.

### Exemples

```csharp
//Démo montrant un cas qui nécessite cette propriété :
[C#]

//Exemple autonome
Workbook workbook = new Workbook("ExternalSourceChart.xlsx");
Worksheet worksheet = workbook.Worksheets[0];
Chart chart = worksheet.Charts[0];
chart.Calculate();
string XValues = chart.NSeries[0].XValues;
// XValues peut être comme "[External.xlsx]Sheet1!$B$2:$C$6" ce qui est compliqué
// pour que l'utilisateur obtienne les valeurs réelles (les valeurs peuvent être liées à un autre classeur,
// ou mis en cache dans le classeur actuel). Ici vous pouvez utiliser la propriété CategoryValues
// pour obtenir les valeurs de catégorie réellement affichées dans l'interface Excel
// sous la forme d'un tableau à deux dimensions.
ChartDataValue[][] v1 = chart.NSeries[0].CategoryValues;

```

### Voir aussi

* class [ChartDataValue](../../chartdatavalue/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


