---
title: "DataLabels.SeparatorValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataLabels-egenskap. Hämtar eller anger separatorvärdet som används för datalabels på ett diagram"
type: docs
url: /sv/net/aspose.cells.charts/datalabels/separatorvalue/
---
## DataLabels.SeparatorValue property

Hämtar eller anger separatorns värde som används för datamärken i ett diagram.

```csharp
public string SeparatorValue { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertySeparatorValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Konfigurera DataLabels
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            dataLabels.ShowValue = true;
            dataLabels.ShowCategoryName = true;
            dataLabels.SeparatorValue = " | "; // Demonstrate SeparatorValue property
            dataLabels.Position = LabelPositionType.Center;

            workbook.Save("DataLabelsSeparatorValueDemo.xlsx");
        }
    }
}
```

### Se även

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


