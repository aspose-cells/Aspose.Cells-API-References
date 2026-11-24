---
title: "TickLabels.RotationAngle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TickLabels-Eigenschaft. Stellt den Textrotationswinkel im Uhrzeigersinn dar"
type: docs
url: /de/net/aspose.cells.charts/ticklabels/rotationangle/
---
## TickLabels.RotationAngle property

Stellt den Textrotationswinkel im Uhrzeigersinn dar.

```csharp
public int RotationAngle { get; set; }
```

### Hinweise

0: Nicht gedreht.255: Von oben nach unten.-90: Nach unten.90: Nach oben.

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["A1"].PutValue("Category 1");
            sheet.Cells["A2"].PutValue("Category 2");
            sheet.Cells["A3"].PutValue("Category 3");
            sheet.Cells["B1"].PutValue(100);
            sheet.Cells["B2"].PutValue(200);
            sheet.Cells["B3"].PutValue(300);

            // Füge ein Diagramm hinzu
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];
            
            // Diagrammdatenquelle festlegen
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Kategorieachsen-Tick-Labels um 45 Grad drehen
            chart.CategoryAxis.TickLabels.RotationAngle = 45;

            // Speichere die Arbeitsmappe
            workbook.Save("TickLabelsRotationDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


