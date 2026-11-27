---
title: "TickLabels.RotationAngle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TickLabels-egenskap. Representerar textens rotationsvinkel medurs"
type: docs
url: /sv/net/aspose.cells.charts/ticklabels/rotationangle/
---
## TickLabels.RotationAngle property

Representerar textens rotationsvinkel medurs.

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
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyRotationAngleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue("Category 1");
            sheet.Cells["A2"].PutValue("Category 2");
            sheet.Cells["A3"].PutValue("Category 3");
            sheet.Cells["B1"].PutValue(100);
            sheet.Cells["B2"].PutValue(200);
            sheet.Cells["B3"].PutValue(300);

            // Lägg till ett diagram
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];
            
            // Ställ in diagramdatakälla
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Rotera kategoriaxelns tick-etiketter med 45 grader
            chart.CategoryAxis.TickLabels.RotationAngle = 45;

            // Spara arbetsboken
            workbook.Save("TickLabelsRotationDemo.xlsx");
        }
    }
}
```

### Se även

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


