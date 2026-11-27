---
title: "DataLabels.BackgroundMode"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataLabels-egenskap. Hämtar och anger bakgrundens visningsläge"
type: docs
url: /sv/net/aspose.cells.charts/datalabels/backgroundmode/
---
## DataLabels.BackgroundMode property

Hämtar och anger visningsläget för bakgrunden

```csharp
public BackgroundMode BackgroundMode { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyBackgroundModeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(5);

            // Skapa ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B3", true);

            // Hämta dataetiketter
            Aspose.Cells.Charts.DataLabels dataLabels = chart.NSeries[0].DataLabels;
            dataLabels.ShowValue = true;

            // Demonstrera egenskapen BackgroundMode
            dataLabels.BackgroundMode = BackgroundMode.Automatic; // Automatic background
            Console.WriteLine("BackgroundMode set to Automatic");

            // Spara arbetsboken
            workbook.Save("DataLabelsBackgroundModeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [BackgroundMode](../../backgroundmode/)
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


