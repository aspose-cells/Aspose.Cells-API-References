---
title: "Chart.Name"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Chart egenskap. Hämtar och anger namnet på diagrammet"
type: docs
url: /sv/net/aspose.cells.charts/chart/name/
---
## Chart.Name property

Hämtar och anger namnet på diagrammet.

```csharp
public string Name { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Visa diagramnamn
            Console.WriteLine("Chart Name: " + chart.Name);

            // Lägg till ett annat diagram och visa dess namn
            int chartIndex2 = worksheet.Charts.Add(ChartType.Pie, 20, 0, 30, 5);
            Aspose.Cells.Charts.Chart chart2 = worksheet.Charts[chartIndex2];
            chart2.NSeries.Add("B2:B4", true);
            chart2.NSeries.CategoryData = "A2:A4";
            Console.WriteLine("Second Chart Name: " + chart2.Name);
        }
    }
}
```

### Se även

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


