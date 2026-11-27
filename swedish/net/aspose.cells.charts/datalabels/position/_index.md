---
title: "DataLabels.Position"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataLabels-egenskap. Representerar positionen för datalabeln"
type: docs
url: /sv/net/aspose.cells.charts/datalabels/position/
---
## DataLabels.Position property

Representerar positionen för datamärket.

```csharp
public LabelPositionType Position { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyPositionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Lägg till ett diagram
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Aktivera datamärkningar
            chart.NSeries[0].DataLabels.ShowValue = true;
            
            // Ställ in position för datalabel
            chart.NSeries[0].DataLabels.Position = LabelPositionType.Right;

            // Spara arbetsboken
            workbook.Save("DataLabelsPositionDemo.xlsx");
        }
    }
}
```

### Se även

* enum [LabelPositionType](../../labelpositiontype/)
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


