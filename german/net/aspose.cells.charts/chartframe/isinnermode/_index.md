---
title: "ChartFrame.IsInnerMode"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartFrame‑Eigenschaft. Gibt an, ob die Größe des Plot‑Bereichs die Tick‑Markierungen und Achsenbeschriftungen einschließt. False bedeutet, dass die Größe den Plot‑Bereich, die Tick‑Markierungen und die Achsenbeschriftungen bestimmt."
type: docs
url: /de/net/aspose.cells.charts/chartframe/isinnermode/
---
## ChartFrame.IsInnerMode property

Gibt an, ob die Größe des Plotbereichs die Tick-Markierungen und Achsenbeschriftungen einschließt. False bedeutet, dass die Größe die Größe des Plotbereichs, der Tick-Markierungen und der Achsenbeschriftungen bestimmt.

```csharp
public bool IsInnerMode { get; set; }
```

### Hinweise

Nur für Xlsx‑Dateien.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyIsInnerModeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Diagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Greife auf den Diagrammrahmen zu und demonstriere IsInnerMode
            Aspose.Cells.Charts.ChartFrame chartFrame = chart.ChartArea;
            chartFrame.IsInnerMode = true; // Set to use inner mode
            
            // Setze einige grundlegende Eigenschaften, um die Wirkung zu zeigen
            chartFrame.Border.Color = Color.Blue;
            chartFrame.Border.Style = Aspose.Cells.Drawing.LineType.Solid;
            chartFrame.Area.ForegroundColor = Color.LightYellow;

            workbook.Save("ChartFrameIsInnerModeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


