---
title: "Enum BubbleSizeRepresents"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.BubbleSizeRepresents-enum. Representerar vad bubblens storlek representerar i ett bubbeldiagram"
type: docs
url: /sv/net/aspose.cells.charts/bubblesizerepresents/
---
## BubbleSizeRepresents enumeration

Representerar vad bubbelns storlek står för i ett bubbeldiagram.

```csharp
public enum BubbleSizeRepresents
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| SizeIsArea | `0` | Representerar värdet av [`BubbleSizes`](../series/bubblesizes/), vilket är bubblans area. |
| SizeIsWidth | `1` | Representerar värdet av [`BubbleSizes`](../series/bubblesizes/) som är bubblans bredd. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class BubbleSizeRepresentsDemo
    {
        public static void BubbleSizeRepresentsExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för bubbeldiagrammet
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["B2"].PutValue(3);
            worksheet.Cells["B3"].PutValue(4);
            worksheet.Cells["C1"].PutValue(5);
            worksheet.Cells["C2"].PutValue(10);
            worksheet.Cells["C3"].PutValue(15);

            // Lägg till ett bubbeldiagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Bubble, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Lägg till serier i bubbeldiagrammet
            int seriesIndex = chart.NSeries.Add("A1:C3", true);
            Series series = chart.NSeries[seriesIndex];

            // Ange X‑värden, Y‑värden och bubbelförstorlekar.
            series.XValues = "A1:A3";
            series.Values = "B1:B3";
            series.BubbleSizes = "C1:C3";

            // Ställ in representationen av bubbelförstoringen.
            series.SizeRepresents = BubbleSizeRepresents.SizeIsArea;

            // Spara arbetsboken
            workbook.Save("BubbleSizeRepresentsExample.xlsx");
            workbook.Save("BubbleSizeRepresentsExample.pdf");

            // Ställ in representationen av bubbelförstoringen.
            series.SizeRepresents = BubbleSizeRepresents.SizeIsWidth;

            // Spara arbetsboken
            workbook.Save("BubbleSizeRepresentsExample2.xlsx");
            workbook.Save("BubbleSizeRepresentsExample2.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


