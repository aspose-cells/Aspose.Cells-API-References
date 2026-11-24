---
title: "TickLabels.DirectionType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TickLabels-Eigenschaft. Liest und setzt die Textausrichtung."
type: docs
url: /de/net/aspose.cells.charts/ticklabels/directiontype/
---
## TickLabels.DirectionType property

Liest und legt die Textausrichtung fest.

```csharp
public ChartTextDirectionType DirectionType { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyDirectionTypeDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].Value = 50;
            worksheet.Cells["A2"].Value = 100;
            worksheet.Cells["A3"].Value = 150;
            worksheet.Cells["A4"].Value = 200;
            worksheet.Cells["B1"].Value = 60;
            worksheet.Cells["B2"].Value = 32;
            worksheet.Cells["B3"].Value = 50;
            worksheet.Cells["B4"].Value = 40;
            worksheet.Cells["C1"].Value = "清华";
            worksheet.Cells["C2"].Value = "北大";
            worksheet.Cells["C3"].Value = "人大";
            worksheet.Cells["C4"].Value = "科大";

            // Diagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Diagrammdaten festlegen
            chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";

            // Setzt die Ausrichtung der TickLabels auf vertikal
            chart.CategoryAxis.TickLabels.DirectionType = ChartTextDirectionType.Vertical;

            // Speichere die Arbeitsmappe
            workbook.Save("TickLabelsDirectionTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [ChartTextDirectionType](../../charttextdirectiontype/)
* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


