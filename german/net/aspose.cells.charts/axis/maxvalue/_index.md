---
title: "Axis.MaxValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Axis-Eigenschaft. Stellt den Maximalwert der Werteachse dar."
type: docs
url: /de/net/aspose.cells.charts/axis/maxvalue/
---
## Axis.MaxValue property

Gibt den Maximalwert auf der Werteachse an.

```csharp
public object MaxValue { get; set; }
```

### Hinweise

Der Typ von maxValue kann nur double oder DateTime sein

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyMaxValueDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(50);

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Setze den Maximalwert der Werteachse
            chart.ValueAxis.MaxValue = 60;

            // Speichere die Arbeitsmappe
            workbook.Save("AxisPropertyMaxValueDemo_out.xlsx");
        }
    }
}
```

### Siehe auch

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


