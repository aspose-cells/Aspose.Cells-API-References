---
title: "Enum BackgroundMode"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.BackgroundMode enum. Representerar bakgrundens visningsläge"
type: docs
url: /sv/net/aspose.cells.charts/backgroundmode/
---
## BackgroundMode enumeration

Representerar bakgrundens visningsläge.

```csharp
public enum BackgroundMode
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Automatic | `0` | Automatisk |
| Opaque | `1` | Opak |
| Transparent | `2` | Transparent |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class BackgroundModeDemo
    {
        public static void BackgroundModeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Hämta referensen till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till lite exempeldata i celler
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            
            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Lägg till NSeries (diagramdatakälla) till diagrammet som sträcker sig från cellen "A1" till "B3"
            chart.NSeries.Add("A1:B3", true);
            
            // Åtkomst till diagramområdet
            ChartArea chartArea = chart.ChartArea;

            // Ställ in förgrundsfärgen för diagramområdet
            chartArea.Area.ForegroundColor = Color.Yellow;

            // Ställ in bakgrundsläget för diagramområdet
            chartArea.BackgroundMode = BackgroundMode.Opaque;
            chartArea.Area.Transparency = 0.8;           
            
            
            // Ställ in skuggan för diagramområdet
            chartArea.Shadow = true;
            
            // Spara arbetsboken
            workbook.Save("BackgroundModeExample.xlsx");
            workbook.Save("BackgroundModeExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


