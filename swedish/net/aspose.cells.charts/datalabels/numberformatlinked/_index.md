---
title: "DataLabels.NumberFormatLinked"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataLabels-egenskap. Sant om talformatet är länkat till cellerna så att talformatet ändras i etiketterna när det ändras i cellerna"
type: docs
url: /sv/net/aspose.cells.charts/datalabels/numberformatlinked/
---
## DataLabels.NumberFormatLinked property

Sant om talformatet är länkat till cellerna (så att talformatet ändras i etiketterna när det ändras i cellerna).

```csharp
public bool NumberFormatLinked { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyNumberFormatLinkedDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["C1"].PutValue("Formatted Value");
            worksheet.Cells["C2"].PutValue("100 units");
            worksheet.Cells["C3"].PutValue("200 units");

            // Skapa ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Lägg till serie
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            
            // Konfigurera datamärkningar
            var series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;
            series.DataLabels.LinkedSource = "C2:C3";
            series.DataLabels.NumberFormatLinked = true; // Link number format from source cells
            
            // Spara arbetsboken
            workbook.Save("DataLabelsNumberFormatLinkedDemo.xlsx");
        }
    }
}
```

### Se även

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


