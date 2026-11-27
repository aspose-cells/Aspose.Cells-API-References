---
title: "SeriesCollection.CategoryData"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SeriesCollection-egenskapen. Hämtar eller anger intervallet för kategori-axelvärden. Det kan vara ett cellintervall såsom d1e10 eller en sekvens av värden såsom 26810"
type: docs
url: /sv/net/aspose.cells.charts/seriescollection/categorydata/
---
## SeriesCollection.CategoryData property

Hämtar eller anger intervallet för kategori‑axelvärden. Det kan vara ett cellintervall (t.ex. "d1:e10") eller en sekvens av värden (t.ex. "{2,6,8,10}").

```csharp
public string CategoryData { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionPropertyCategoryDataDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue("Cat " + (i - 1));
                worksheet.Cells["B" + i].PutValue(i * 10);
            }
            
            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("=Sheet1!$B$2:$B$10", true);
            chart.NSeries.CategoryData = "=Sheet1!$A$2:$A$10";
            
            // Spara arbetsboken
            workbook.Save("CategoryDataDemo.xlsx");
            
            // Verifiera CategoryData-egenskapen
            Console.WriteLine("Chart CategoryData: " + chart.NSeries.CategoryData);
        }
    }
}
```

### Se även

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


