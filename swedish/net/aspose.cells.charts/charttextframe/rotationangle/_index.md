---
title: "ChartTextFrame.RotationAngle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartTextFrame-egenskap. Representerar textens rotationsvinkel"
type: docs
url: /sv/net/aspose.cells.charts/charttextframe/rotationangle/
---
## ChartTextFrame.RotationAngle property

Representerar textrotationsvinkeln.

```csharp
public int RotationAngle { get; set; }
```

### Anmärkningar

0: Inte roterad.255: Toppen till botten.-90: Nedåt.90: Uppåt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyRotationAngleDemo
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

            // Lägg till ett diagram och ange dess dataintervall
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ställ in rotationsvinkel för värdeaxelns titel
            chart.ValueAxis.Title.Text = "Values";
            chart.ValueAxis.Title.RotationAngle = 45;

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


