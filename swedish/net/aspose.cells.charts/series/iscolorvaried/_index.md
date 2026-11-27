---
title: "Series.IsColorVaried"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Series-egenskap. Representerar om färgen på punkterna varierar. Diagrammet måste innehålla endast en serie eller så är detta diagram ett pajdiagram"
type: docs
url: /sv/net/aspose.cells.charts/series/iscolorvaried/
---
## Series.IsColorVaried property

Representerar om färgen på punkterna varierar. Diagrammet måste innehålla endast en serie eller så är diagrammet ett cirkeldiagram.

```csharp
public bool IsColorVaried { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyIsColorVariedDemo
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
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ställ in IsColorVaried-egenskapen för den första serien
            chart.NSeries[0].IsColorVaried = true;

            // Spara arbetsboken
            workbook.Save("output.xlsx");

            // Verifiera egenskapen
            Console.WriteLine("IsColorVaried: " + chart.NSeries[0].IsColorVaried);
        }
    }
}
```

### Se även

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


