---
title: "Axis.IsPlotOrderReversed"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Axis. Indique si Microsoft Excel trace les points de données du dernier au premier"
type: docs
url: /fr/net/aspose.cells.charts/axis/isplotorderreversed/
---
## Axis.IsPlotOrderReversed property

Représente si Microsoft Excel trace les points de données du dernier au premier.

```csharp
public bool IsPlotOrderReversed { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyIsPlotOrderReversedDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["A3"].PutValue("Category 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // Ajouter un graphique en colonnes
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Définir la source de données du graphique
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Inverser l'ordre d'affichage des catégories
            chart.CategoryAxis.IsPlotOrderReversed = true;

            // Enregistrez le classeur
            workbook.Save("AxisPropertyIsPlotOrderReversedDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


