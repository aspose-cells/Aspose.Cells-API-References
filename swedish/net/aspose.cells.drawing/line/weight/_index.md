---
title: "Line.Weight"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Linjeegenskap. Hämtar eller anger WeightType för linjen"
type: docs
url: /sv/net/aspose.cells.drawing/line/weight/
---
## Line.Weight property

Hämtar eller anger [`WeightType`](../../weighttype/) för linjen.

```csharp
public WeightType Weight { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyWeightDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Åtkomst till diagramområdet och ställ in kantens tjocklek
            ChartArea chartArea = chart.ChartArea;
            chartArea.Border.Weight = WeightType.MediumLine;

            // Spara arbetsboken
            workbook.Save("LinePropertyWeightDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* enum [WeightType](../../weighttype/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


