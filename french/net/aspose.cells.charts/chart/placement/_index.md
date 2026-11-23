---
title: "Chart.Placement"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Chart. Représente la façon dont le graphique est attaché aux cellules en dessous"
type: docs
url: /fr/net/aspose.cells.charts/chart/placement/
---
## Chart.Placement property

Représente la façon dont le graphique est attaché aux cellules en dessous.

```csharp
public PlacementType Placement { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPropertyPlacementDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ajoutez un graphique et définissez les données
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Démontrer la propriété Placement
            chart.Placement = PlacementType.MoveAndSize;
            Console.WriteLine("Chart Placement: " + chart.Placement);

            workbook.Save("ChartPlacementDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [PlacementType](../../../aspose.cells.drawing/placementtype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


