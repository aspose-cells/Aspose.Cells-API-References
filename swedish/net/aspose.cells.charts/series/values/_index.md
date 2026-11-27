---
title: "Series.Values"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Series‑egenskap. Representerar Y‑värdena för denna diagramserie"
type: docs
url: /sv/net/aspose.cells.charts/series/values/
---
## Series.Values property

Representerar Y‑värdena för denna diagramserie.

```csharp
public string Values { get; set; }
```

### Anmärkningar

För att hämta de faktiska värdena (motsvarande varje punkt i denna serie) som definieras av denna egenskap, använd [`PointValues`](../pointvalues/).

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyValuesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i celler
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["C1"].PutValue("Series2");
            
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            
            worksheet.Cells["C2"].PutValue(15);
            worksheet.Cells["C3"].PutValue(25);
            worksheet.Cells["C4"].PutValue(35);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Lägg till serie med Values‑egenskapen
            chart.NSeries.Add("=Sheet1!$B$2:$B$4", true);
            chart.NSeries.Add("=Sheet1!$C$2:$C$4", true);

            // Ange kategoridata
            chart.NSeries.CategoryData = "=Sheet1!$A$2:$A$4";

            // Visa Values‑egenskapen för varje serie
            Console.WriteLine("Series 1 Values: " + chart.NSeries[0].Values);
            Console.WriteLine("Series 2 Values: " + chart.NSeries[1].Values);

            // Spara arbetsboken
            workbook.Save("SeriesPropertyValuesDemo.xlsx");
        }
    }
}
```

### Se även

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


