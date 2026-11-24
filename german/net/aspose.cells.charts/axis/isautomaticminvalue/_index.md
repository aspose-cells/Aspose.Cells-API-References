---
title: "Axis.IsAutomaticMinValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Axis-Eigenschaft. Gibt an, ob der Minimalwert automatisch zugewiesen wird"
type: docs
url: /de/net/aspose.cells.charts/axis/isautomaticminvalue/
---
## Axis.IsAutomaticMinValue property

Gibt an, ob der Minimalwert automatisch zugewiesen wird.

```csharp
public bool IsAutomaticMinValue { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyIsAutomaticMinValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // Diagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Werteachse konfigurieren
            Axis valueAxis = chart.ValueAxis;
            valueAxis.IsAutomaticMinValue = false;
            valueAxis.MinValue = 0;
            valueAxis.IsAutomaticMaxValue = true; // Keep max value automatic for contrast
            
            // Ergebnis speichern
            workbook.Save("AxisPropertyIsAutomaticMinValueDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


