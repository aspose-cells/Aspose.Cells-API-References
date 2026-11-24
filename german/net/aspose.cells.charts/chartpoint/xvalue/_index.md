---
title: "ChartPoint.XValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartPoint-Eigenschaft. Gibt den X‑Wert des Diagrammpunkts zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells.charts/chartpoint/xvalue/
---
## ChartPoint.XValue property

Liest oder setzt den X‑Wert des Diagrammpunkts.

```csharp
public object XValue { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPointPropertyXValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten hinzufügen
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["A3"].PutValue("Category 3");
            worksheet.Cells["B1"].PutValue(50);
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(150);

            // Ein Diagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Festlegen der Diagrammdatenquelle
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Anpassen von Datenpunkten
            for (int i = 0; i < chart.NSeries[0].Points.Count; i++)
            {
                ChartPoint point = chart.NSeries[0].Points[i];
                
                // Demonstration der Verwendung der XValue‑Eigenschaft
                point.XValue = "Modified " + (i + 1);
                
                // Zusätzliche Formatierung zur Sichtbarkeit
                point.Area.ForegroundColor = Color.FromArgb(100 + i * 50, 150, 200);
            }

            workbook.Save("ChartPointXValueDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


