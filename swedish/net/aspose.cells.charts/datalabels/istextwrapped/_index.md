---
title: "DataLabels.IsTextWrapped"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataLabels-egenskap. Hämtar eller anger ett värde som indikerar om texten är radbruten"
type: docs
url: /sv/net/aspose.cells.charts/datalabels/istextwrapped/
---
## DataLabels.IsTextWrapped property

Hämtar eller anger ett värde som indikerar om texten är radbruten.

```csharp
public override bool IsTextWrapped { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyIsTextWrappedDemo
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
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(120);
            worksheet.Cells["B3"].PutValue(85);
            worksheet.Cells["B4"].PutValue(65);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Åtkomst till datamärkningar
            Aspose.Cells.Charts.DataLabels labels = chart.NSeries[0].DataLabels;
            
            // Visa dataetiketter
            labels.ShowValue = true;
            
            // Demonstrera IsTextWrapped-egenskapen
            Console.WriteLine("Before setting IsTextWrapped: " + labels.IsTextWrapped);
            labels.IsTextWrapped = true;
            Console.WriteLine("After setting IsTextWrapped: " + labels.IsTextWrapped);

            // Spara arbetsboken
            workbook.Save("DataLabels_IsTextWrapped_Demo.xlsx");
        }
    }
}
```

### Se även

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


