---
title: "ChartFrame.Border"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartFrame-Eigenschaft. Gibt den Rand zurück"
type: docs
url: /de/net/aspose.cells.charts/chartframe/border/
---
## ChartFrame.Border property

Gibt den [`border`](../../../aspose.cells.drawing/line/) zurück.

```csharp
public virtual Line Border { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyBorderDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten zum Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Ein Säulendiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Auf Diagrammtitel zugreifen
            chart.Title.Text = "Chart Title with Custom Border";
            ChartFrame title = chart.Title;

            // Rand‑Eigenschaften konfigurieren
            Line border = title.Border;
            border.Color = System.Drawing.Color.Red;
            border.Style = LineType.Solid;
            border.Weight = WeightType.MediumLine;
            border.Transparency = 0.3;
            border.DashType = MsoLineDashStyle.Solid;

            // Ergebnis speichern
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Line](../../../aspose.cells.drawing/line/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


