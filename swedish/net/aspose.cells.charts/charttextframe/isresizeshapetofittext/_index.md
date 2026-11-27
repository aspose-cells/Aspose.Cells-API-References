---
title: "ChartTextFrame.IsResizeShapeToFitText"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartTextFrame-egenskap. Hämtar eller anger om en form ska anpassas automatiskt för att helt innehålla den beskrivna texten. Automatisk anpassning innebär att texten i en form skalas för att rymma all text"
type: docs
url: /sv/net/aspose.cells.charts/charttextframe/isresizeshapetofittext/
---
## ChartTextFrame.IsResizeShapeToFitText property

Hämtar eller anger om en form ska automatiskt anpassas för att helt innehålla den beskrivna texten. Automatisk anpassning innebär att texten i en form skalas för att rymma all text.

```csharp
public bool IsResizeShapeToFitText { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyIsResizeShapeToFitTextDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook(FileFormatType.Xlsx);
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["A3"].PutValue("Category 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // Lägg till ett stapeldiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange seriedata
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Åtkomst till datamärkningar
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            dataLabels.ShowValue = true;
            dataLabels.Position = LabelPositionType.Center;

            // Demonstrera IsResizeShapeToFitText-egenskapen
            foreach (ChartPoint point in chart.NSeries[0].Points)
            {
                // Inaktivera automatisk storleksändring av form för att passa text
                point.DataLabels.IsResizeShapeToFitText = false;
                
                // Ställ in anpassad bredd som är mindre än vad texten normalt skulle kräva
                point.DataLabels.Width = 50;
            }

            // Spara arbetsboken
            workbook.Save("ChartTextFramePropertyIsResizeShapeToFitTextDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


