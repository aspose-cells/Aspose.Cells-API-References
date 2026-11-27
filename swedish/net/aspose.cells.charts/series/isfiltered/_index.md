---
title: "Series.IsFiltered"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Series-egenskap. Anger om serien är markerad eller filtrerad. True betyder att serien är filtrerad och den kommer inte att visas i diagrammet"
type: docs
url: /sv/net/aspose.cells.charts/series/isfiltered/
---
## Series.IsFiltered property

Anger om serien är markerad eller filtrerad. Sant indikerar att serien är filtrerad och den kommer inte att visas i diagrammet.

```csharp
public bool IsFiltered { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyIsFilteredDemo
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
            worksheet.Cells["A5"].PutValue("D");
            
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);
            
            worksheet.Cells["C1"].PutValue("Series2");
            worksheet.Cells["C2"].PutValue(15);
            worksheet.Cells["C3"].PutValue(25);
            worksheet.Cells["C4"].PutValue(35);
            worksheet.Cells["C5"].PutValue(45);
            
            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.Add("C2:C5", true);
            chart.NSeries.CategoryData = "A2:A5";
            
            // Demonstrera egenskapen IsFiltered
            Console.WriteLine("Initial Series Count: " + chart.NSeries.Count);
            
            // Filtrera den första serien
            chart.NSeries[0].IsFiltered = true;
            Console.WriteLine("After filtering first series: " + chart.NSeries.Count);
            
            // Filtrera den andra serien
            chart.NSeries[0].IsFiltered = true;
            Console.WriteLine("After filtering second series: " + chart.NSeries.Count);
            
            // Spara arbetsboken
            workbook.Save("SeriesFilteredDemo_out.xlsx");
        }
    }
}
```

### Se även

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


