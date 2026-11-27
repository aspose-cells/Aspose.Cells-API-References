---
title: "TickLabels.ReadingOrder"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TickLabels‑egenskap. Representerar textens läsriktning"
type: docs
url: /sv/net/aspose.cells.charts/ticklabels/readingorder/
---
## TickLabels.ReadingOrder property

Representerar textens läsriktning.

```csharp
public TextDirectionType ReadingOrder { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyReadingOrderDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);

            // Ange tick‑etiketternas läsriktning
            TickLabels tickLabels = chart.ValueAxis.TickLabels;
            tickLabels.ReadingOrder = TextDirectionType.RightToLeft;

            // Spara arbetsboken
            workbook.Save("TickLabelsReadingOrderDemo.xlsx");
        }
    }
}
```

### Se även

* enum [TextDirectionType](../../../aspose.cells/textdirectiontype/)
* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


