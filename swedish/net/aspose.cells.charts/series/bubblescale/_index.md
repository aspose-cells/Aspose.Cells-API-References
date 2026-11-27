---
title: "Series.BubbleScale"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Series-egenskap. Hämtar eller anger skalningsfaktorn för bubblor i den angivna diagramgruppen. Det kan vara ett heltal från 0 till 300 som motsvarar en procentsats av standardstorleken. Gäller endast för bubbeldiagram"
type: docs
url: /sv/net/aspose.cells.charts/series/bubblescale/
---
## Series.BubbleScale property

Hämtar eller anger skalningsfaktorn för bubblor i den angivna diagramgruppen. Den kan vara ett heltal mellan 0 (noll) och 300, motsvarande en procentsats av standardstorleken. Gäller endast för bubbeldiagram.

```csharp
public int BubbleScale { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SeriesPropertyBubbleScaleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för bubbeldiagram
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["B1"].PutValue("Y");
            worksheet.Cells["C1"].PutValue("Size");
            
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["C2"].PutValue(5);
            
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["C3"].PutValue(10);
            
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["C4"].PutValue(15);

            // Lägg till ett bubbeldiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Bubble, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Lägg till serier i diagrammet
            int seriesIndex = chart.NSeries.Add("B2:B4", true);
            chart.NSeries[seriesIndex].XValues = "A2:A4";
            chart.NSeries[seriesIndex].BubbleSizes = "C2:C4";
            
            // Ställ in bubblskalning för att demonstrera egenskapen
            chart.NSeries[seriesIndex].BubbleScale = 150; // Scale bubbles to 150% of default size
            
            // Anpassa diagrammets utseende
            chart.Title.Text = "Bubble Chart with Scaled Bubbles";
            chart.NSeries[seriesIndex].Area.FillFormat.SetOneColorGradient(Color.LightBlue, 0.5, Aspose.Cells.Drawing.GradientStyleType.Horizontal, 1);
            
            // Spara arbetsboken
            workbook.Save("BubbleScaleDemo.xlsx");
        }
    }
}
```

### Se även

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


