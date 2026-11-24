---
title: "Axis.CustomDisplayUnit"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Axis-Eigenschaft. Gibt einen benutzerdefinierten Wert für die Anzeigeeinheit an."
type: docs
url: /de/net/aspose.cells.charts/axis/customdisplayunit/
---
## Axis.CustomDisplayUnit property

Gibt einen benutzerdefinierten Wert für die Anzeigeeinheit an.

```csharp
public double CustomDisplayUnit { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyCustomDisplayUnitDemo
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
            worksheet.Cells["B2"].PutValue(10000000);
            worksheet.Cells["B3"].PutValue(20000000);
            worksheet.Cells["B4"].PutValue(30000000);

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenquelle festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Benutzerdefinierte Anzeigeeinheit für die Werteachse festlegen
            chart.ValueAxis.CustomDisplayUnit = 1.0E7;
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Custom;
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


