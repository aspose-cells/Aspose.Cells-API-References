---
title: "PlotArea.IsAutomaticSize"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PlotArea. Indique si la zone de tracé est dimensionnée automatiquement"
type: docs
url: /fr/net/aspose.cells.charts/plotarea/isautomaticsize/
---
## PlotArea.IsAutomaticSize property

Indique si la zone de tracé est dimensionnée automatiquement.

```csharp
public override bool IsAutomaticSize { get; set; }
```

### Remarques

NOTE : lorsque IsAutomaticSize est défini sur True, les valeurs que vous avez définies manuellement pour la largeur et la hauteur seront désactivées.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PlotAreaPropertyIsAutomaticSizeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Ajouter un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Configurer la zone de tracé
            PlotArea plotArea = chart.PlotArea;
            plotArea.IsAutomaticSize = false; // Disable automatic sizing
            plotArea.Width = 3000;
            plotArea.Height = 2000;

            workbook.Save("PlotAreaIsAutomaticSizeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


