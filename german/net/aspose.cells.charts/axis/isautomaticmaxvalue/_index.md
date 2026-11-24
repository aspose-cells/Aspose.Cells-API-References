---
title: "Axis.IsAutomaticMaxValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Axis-Eigenschaft. Gibt an, ob der Maximalwert automatisch zugewiesen wird"
type: docs
url: /de/net/aspose.cells.charts/axis/isautomaticmaxvalue/
---
## Axis.IsAutomaticMaxValue property

Gibt an, ob der Maximalwert automatisch zugewiesen wird.

```csharp
public bool IsAutomaticMaxValue { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyIsAutomaticMaxValueDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
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

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenquelle festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Hole die Werte-Achse
            Axis valueAxis = chart.ValueAxis;

            // Demonstration der IsAutomaticMaxValue‑Eigenschaft
            Console.WriteLine("Initial IsAutomaticMaxValue: " + valueAxis.IsAutomaticMaxValue);
            Console.WriteLine("Initial MaxValue: " + valueAxis.MaxValue);

            // Automatischen Maximalwert deaktivieren und benutzerdefinierten Wert festlegen
            valueAxis.IsAutomaticMaxValue = false;
            valueAxis.MaxValue = 40;
            Console.WriteLine("After change - IsAutomaticMaxValue: " + valueAxis.IsAutomaticMaxValue);
            Console.WriteLine("After change - MaxValue: " + valueAxis.MaxValue);

            // Automatischen Maximalwert wieder aktivieren
            valueAxis.IsAutomaticMaxValue = true;
            Console.WriteLine("After re-enabling - IsAutomaticMaxValue: " + valueAxis.IsAutomaticMaxValue);
            Console.WriteLine("After re-enabling - MaxValue: " + valueAxis.MaxValue);

            // Speichere die Arbeitsmappe
            workbook.Save("AxisPropertyIsAutomaticMaxValueDemo_out.xlsx");
        }
    }
}
```

### Siehe auch

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


