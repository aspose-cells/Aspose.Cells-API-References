---
title: "Line.EndType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Line. Spécifie une pointe de flèche pour la fin d'une ligne"
type: docs
url: /fr/net/aspose.cells.drawing/line/endtype/
---
## Line.EndType property

Spécifie une pointe de flèche pour la fin d'une ligne.

```csharp
public MsoArrowheadStyle EndType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyEndTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);

            // Ajouter un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B4", true);

            // Ajouter une ligne de tendance et définir EndType
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Aspose.Cells.Charts.Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.EndType = MsoArrowheadStyle.Arrow;
            trendline.EndArrowLength = MsoArrowheadLength.Medium;
            trendline.EndArrowWidth = MsoArrowheadWidth.Medium;

            workbook.Save("LineEndTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [MsoArrowheadStyle](../../msoarrowheadstyle/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


