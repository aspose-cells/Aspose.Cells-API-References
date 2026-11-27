---
title: "DataLabels.Number"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataLabels-egenskap. Hämtar och anger det inbyggda talformatet"
type: docs
url: /sv/net/aspose.cells.charts/datalabels/number/
---
## DataLabels.Number property

Hämtar och anger det inbyggda talformatet.

```csharp
public int Number { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyNumberDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Bar, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Hämta den första serien och aktivera dataetiketter
            Series series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;
            
            // Åtkomst till egenskaper för dataetiketter
            DataLabels dataLabels = series.DataLabels;
            
            // Demonstrera användning av egenskapen Number
            Console.WriteLine("Original Number format: " + dataLabels.NumberFormat);
            Console.WriteLine("Original Number property value: " + dataLabels.Number);
            
            // Ändra talformatet
            dataLabels.Number = 2; // Currency format
            dataLabels.NumberFormat = "$#,##0.00";
            
            Console.WriteLine("Modified Number format: " + dataLabels.NumberFormat);
            Console.WriteLine("Modified Number property value: " + dataLabels.Number);

            // Spara arbetsboken
            workbook.Save("DataLabelsNumberDemo.xlsx");
        }
    }
}
```

### Se även

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


