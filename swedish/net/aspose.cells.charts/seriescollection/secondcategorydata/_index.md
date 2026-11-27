---
title: "SeriesCollection.SecondCategoryData"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SeriesCollection-egenskapen. Hämtar eller anger intervallet för andra kategori-axelvärden. Det kan vara ett cellintervall såsom d1e10 eller en sekvens av värden såsom 26810. Påverkar endast när vissa serier har plottats på den andra axeln."
type: docs
url: /sv/net/aspose.cells.charts/seriescollection/secondcategorydata/
---
## SeriesCollection.SecondCategoryData property

Hämtar eller anger intervallet för den andra kategori‑axelns värden. Det kan vara ett cellintervall (t.ex. "d1:e10") eller en sekvens av värden (t.ex. "{2,6,8,10}"). Påverkar endast när vissa serier har plottats på den andra axeln.

```csharp
public string SecondCategoryData { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionPropertySecondCategoryDataDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Primary Categories");
            worksheet.Cells["A2"].PutValue("Cat1");
            worksheet.Cells["A3"].PutValue("Cat2");
            worksheet.Cells["A4"].PutValue("Cat3");
            
            worksheet.Cells["B1"].PutValue("Secondary Categories");
            worksheet.Cells["B2"].PutValue("SubCat1");
            worksheet.Cells["B3"].PutValue("SubCat2");
            worksheet.Cells["B4"].PutValue("SubCat3");
            
            worksheet.Cells["C1"].PutValue("Values");
            worksheet.Cells["C2"].PutValue(10);
            worksheet.Cells["C3"].PutValue(20);
            worksheet.Cells["C4"].PutValue(30);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange seriedata
            chart.NSeries.Add("C2:C4", true);
            
            // Ange primär kategoridata
            chart.NSeries.CategoryData = "A2:A4";
            
            // Ange sekundär kategoridata
            chart.NSeries.SecondCategoryData = "B2:B4";

            // Spara arbetsboken
            workbook.Save("SecondCategoryDataDemo.xlsx");
        }
    }
}
```

### Se även

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


