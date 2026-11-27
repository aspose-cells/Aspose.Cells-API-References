---
title: "Series.Area"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Series‑egenskap. Representerar bakgrundsområdet för Series‑objektet"
type: docs
url: /sv/net/aspose.cells.charts/series/area/
---
## Series.Area property

Representerar bakgrundsområdet för Series-objektet.

```csharp
public Area Area { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SeriesPropertyAreaDemo
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

            // Åtkomst till den första serien och ange områdestextur
            Series series = chart.NSeries[0];
            series.Area.FillFormat.Texture = TextureType.Stationery;

            // Spara arbetsboken
            workbook.Save("SeriesPropertyAreaDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [Area](../../../aspose.cells.drawing/area/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


