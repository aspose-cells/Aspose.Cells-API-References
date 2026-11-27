---
title: "Line.WeightPt"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Line-egenskap. Hämtar eller anger linjens vikt i enheten punkter"
type: docs
url: /sv/net/aspose.cells.drawing/line/weightpt/
---
## Line.WeightPt property

Hämtar eller anger linjens tjocklek i enheter av punkter.

```csharp
public double WeightPt { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyWeightPtDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Pie, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Konfigurera datamärkningar
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;
            series.HasLeaderLines = true;

            // Anpassa ledarlinjer
            series.LeaderLines.IsAuto = false;
            series.LeaderLines.Style = Aspose.Cells.Drawing.LineType.Dot;
            series.LeaderLines.WeightPt = 0.25; // Demonstrate WeightPt property
            series.LeaderLines.Color = Color.LightCyan;

            // Spara arbetsboken
            workbook.Save("LeaderLinesDemo.xlsx");
        }
    }
}
```

### Se även

* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


