---
title: "Enum PrintSizeType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.PrintSizeType‑enum. Representerar den utskrivna diagramstorleken"
type: docs
url: /sv/net/aspose.cells/printsizetype/
---
## PrintSizeType enumeration

Representerar den utskrivna diagramstorleken.

```csharp
public enum PrintSizeType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Full | `0` | Använd hel sida. |
| Fit | `1` | Skala för att passa sidan. |
| Custom | `2` | Anpassad. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PrintSizeTypeDemo
    {
        public static void PrintSizeTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            // Hämta det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            worksheet.Cells[0, 0].PutValue("Category");
            worksheet.Cells[0, 1].PutValue("Value");
            worksheet.Cells[1, 0].PutValue("A");
            worksheet.Cells[1, 1].PutValue(10);
            worksheet.Cells[2, 0].PutValue("B");
            worksheet.Cells[2, 1].PutValue(20);
            worksheet.Cells[3, 0].PutValue("C");
            worksheet.Cells[3, 1].PutValue(30);

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange dataintervallet för diagrammet
            chart.SetChartDataRange("A1:B4", true);

            // Ange diagramtitel
            chart.Title.Text = "Sample Chart";

            // Ange utskriftsstorleken för diagrammet
            chart.PrintSize = PrintSizeType.Fit;

            // Spara arbetsboken
            workbook.Save("PrintSizeTypeExample.xlsx");

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


