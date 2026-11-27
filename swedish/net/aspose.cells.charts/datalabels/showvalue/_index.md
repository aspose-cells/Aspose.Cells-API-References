---
title: "DataLabels.ShowValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataLabels-egenskap. Representerar ett specificerat diagram's datalabelvärdesvisningsbeteende. True visar värdena. False döljer dem."
type: docs
url: /sv/net/aspose.cells.charts/datalabels/showvalue/
---
## DataLabels.ShowValue property

Representerar ett specificerat diagrammets dataetiketts värdevisningsbeteende. True visar värdena. False för att dölja.

```csharp
public bool ShowValue { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyShowValueDemo
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

            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Aktivera datalabels och visa värden
            chart.NSeries[0].DataLabels.ShowValue = true;
            chart.NSeries[0].DataLabels.Position = LabelPositionType.Center;

            // Spara arbetsboken
            workbook.Save("DataLabelsShowValueDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


