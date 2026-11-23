---
title: "Axis.MinorTickMark"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Axis. Représente le type de petite marque de graduation pour l'axe spécifié"
type: docs
url: /fr/net/aspose.cells.charts/axis/minortickmark/
---
## Axis.MinorTickMark property

Représente le type de repère mineur pour l'axe spécifié.

```csharp
public TickMarkType MinorTickMark { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyMinorTickMarkDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Données d'exemple
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // Créer un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Configurer les propriétés de l'axe
            Axis valueAxis = chart.ValueAxis;
            valueAxis.MinorTickMark = TickMarkType.Inside;
            valueAxis.MajorTickMark = TickMarkType.Cross;
            valueAxis.MinValue = 0;
            valueAxis.MaxValue = 200;
            valueAxis.MajorUnit = 25;

            workbook.Save("AxisMinorTickMarkDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [TickMarkType](../../tickmarktype/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


