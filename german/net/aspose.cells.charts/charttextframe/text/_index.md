---
title: "ChartTextFrame.Text"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartTextFrame-Eigenschaft. Gibt den Text des Titels eines Frames zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells.charts/charttextframe/text/
---
## ChartTextFrame.Text property

Liest oder legt den Text des Rahmentitels fest.

```csharp
public virtual string Text { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyTextDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Category");
            cells["A2"].PutValue("A");
            cells["A3"].PutValue("B");
            cells["A4"].PutValue("C");
            cells["B1"].PutValue("Value");
            cells["B2"].PutValue(10);
            cells["B3"].PutValue(20);
            cells["B4"].PutValue(30);

            // Diagramm hinzufügen
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Diagrammtiteltext festlegen
            chart.Title.Text = "Sample Chart Title";

            // Legendentext abrufen und ändern
            Legend legend = chart.Legend;
            legend.Text = "Custom Legend Text";

            // Speichere die Arbeitsmappe
            workbook.Save("ChartTextDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


