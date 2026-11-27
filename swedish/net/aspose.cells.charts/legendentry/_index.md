---
title: "Klass LegendEntry"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.LegendEntry-klass. Representerar ett legendpost i ett diagramlegend"
type: docs
url: /sv/net/aspose.cells.charts/legendentry/
---
## LegendEntry class

Representerar en förklaringspost i en diagramförklaring.

```csharp
public class LegendEntry
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AutoScaleFont](../../aspose.cells.charts/legendentry/autoscalefont/) { get; set; } | Sant om texten i objektet ändrar teckenstorlek när objektets storlek ändras. Standardvärdet är Sant. |
| [Background](../../aspose.cells.charts/legendentry/background/) { get; set; } | (**Obsolete.**) Hämtar och anger visningsläget för bakgrunden |
| [BackgroundMode](../../aspose.cells.charts/legendentry/backgroundmode/) { get; set; } | Hämtar och anger visningsläget för bakgrunden |
| [Font](../../aspose.cells.charts/legendentry/font/) { get; } | Hämtar ett [`Font`](./font/)‑objekt för det angivna ChartFrame‑objektet. |
| [IsDeleted](../../aspose.cells.charts/legendentry/isdeleted/) { get; set; } | Hämtar och anger om legendposten är borttagen. |
| [IsTextNoFill](../../aspose.cells.charts/legendentry/istextnofill/) { get; set; } | Hämtar eller anger ingen fyllning av texten. |
| virtual [TextFont](../../aspose.cells.charts/legendentry/textfont/) { get; } | (**Obsolete.**) Hämtar ett [`Font`](./font/)‑objekt för det angivna LegendEntry‑objektet. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class LegendEntryDemo
    {
        public static void LegendEntryExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Lägg till NSeries (diagramdatakälla) till diagrammet från cellen "A1" till "B4"
            chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";

            // Åtkomst till legendposten för den första serien
            LegendEntry legendEntry = chart.NSeries[0].LegendEntry;

            // Ställ in egenskaper för legendposten
            legendEntry.IsDeleted = false;
            legendEntry.IsTextNoFill = false;
            legendEntry.AutoScaleFont = true;
            legendEntry.Background = BackgroundMode.Transparent;
            legendEntry.BackgroundMode = BackgroundMode.Opaque;

            // Åtkomst till och ändra teckensnittet för legendposten
            Font font = legendEntry.Font;
            font.Name = "Arial";
            font.Size = 12;
            font.IsBold = true;
            font.Color = System.Drawing.Color.Blue;

            // Spara arbetsboken
            workbook.Save("LegendEntryExample.xlsx");
            workbook.Save("LegendEntryExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


