---
title: "DataLabels.ShowCategoryName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataLabels-egenskap. Representerar ett specificerat diagramdataetikettkategori-namnvisningsbeteende. Sant för att visa kategorinamnet för dataetiketterna på ett diagram. Falskt för att dölja"
type: docs
url: /sv/net/aspose.cells.charts/datalabels/showcategoryname/
---
## DataLabels.ShowCategoryName property

Representerar ett specificerat diagrammets visningsbeteende för datamärkets kategorinamn. Sant för att visa kategorinamnet för datamärken i ett diagram. Falskt för att dölja.

```csharp
public bool ShowCategoryName { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyShowCategoryNameDemo
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

            // Lägg till ett stapeldiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Aktivera dataetiketter och sätt egenskaper
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            dataLabels.ShowValue = true;
            dataLabels.ShowCategoryName = true;
            dataLabels.SeparatorType = DataLabelsSeparatorType.Semicolon;

            // Spara arbetsboken
            workbook.Save("DataLabelsShowCategoryNameDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


