---
title: "DataLabels.Font"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataLabels-egenskap. Hämtar teckensnittet för DataLabels"
type: docs
url: /sv/net/aspose.cells.charts/datalabels/font/
---
## DataLabels.Font property

Hämtar teckensnittet för DataLabels;

```csharp
public override Font Font { get; }
```

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyFontDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Aktivera datamärkningar
            Aspose.Cells.Charts.DataLabels dataLabels = chart.NSeries[0].DataLabels;
            dataLabels.ShowValue = true;

            // Ställ in teckensnittsegenskaper
            dataLabels.Font.Color = Color.Red;
            dataLabels.Font.Size = 14;
            dataLabels.Font.IsBold = true;
            dataLabels.Font.Name = "Arial";

            // Spara arbetsboken
            workbook.Save("DataLabelsFontDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [Font](../../../aspose.cells/font/)
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


