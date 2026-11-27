---
title: "Series.Smooth"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Series‑egenskap. Representerar kurvutjämning. Sant om kurvutjämning är aktiverad för linjediagrammet eller spridningsdiagrammet. Gäller endast för linjediagram och spridningsdiagram med linjer"
type: docs
url: /sv/net/aspose.cells.charts/series/smooth/
---
## Series.Smooth property

Representerar kurvutjämning. Sant om kurvutjämning är aktiverad för linjediagram eller spridningsdiagram. Gäller endast linjediagram och spridningsdiagram med linjer.

```csharp
public bool Smooth { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertySmoothDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ställ in Smooth-egenskapen för den första serien
            chart.NSeries[0].Smooth = true;

            // Spara arbetsboken
            workbook.Save("SmoothPropertyDemo.xlsx");
        }
    }
}
```

### Se även

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


