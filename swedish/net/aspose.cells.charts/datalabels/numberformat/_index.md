---
title: "DataLabels.NumberFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataLabels-egenskap. Representerar formatsträngen för DataLabels-objektet"
type: docs
url: /sv/net/aspose.cells.charts/datalabels/numberformat/
---
## DataLabels.NumberFormat property

Representerar formatsträngen för DataLabels-objektet.

```csharp
public string NumberFormat { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyNumberFormatDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Aktivera datamärkningar
            Series series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;
            
            // Ange anpassat talformat för dataetiketter
            series.DataLabels.NumberFormat = "_(* #,##0_);_(* \\(#,##0\\);_(* \"-\"??_);_(@_)";
            
            // Spara arbetsboken
            workbook.Save("DataLabelsNumberFormatDemo.xlsx");
        }
    }
}
```

### Se även

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


