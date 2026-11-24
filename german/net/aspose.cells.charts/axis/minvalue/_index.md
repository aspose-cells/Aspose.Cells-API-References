---
title: "Axis.MinValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Achsen-Eigenschaft. Stellt den Minimalwert auf der Werteachse dar"
type: docs
url: /de/net/aspose.cells.charts/axis/minvalue/
---
## Axis.MinValue property

Gibt den Minimalwert auf der Werteachse an.

```csharp
public object MinValue { get; set; }
```

### Hinweise

Der minValue-Typ kann nur double oder DateTime sein

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyMinValueDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu und füge Beispieldaten hinzu
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["B1"].PutValue(40);
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(60);

            // Füge ein Diagramm hinzu und setze den Datenbereich
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 5, 15, 15);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B3", false);

            // Werteachsen-Eigenschaften konfigurieren
            chart.ValueAxis.MinValue = 15;  // Setting minimum value
            chart.ValueAxis.MaxValue = 70;
            chart.ValueAxis.MajorUnit = 10;

            // Speichere die Arbeitsmappe
            workbook.Save("AxisMinValueDemo.xlsx");

            Console.WriteLine("Chart created with MinValue set to 15.");
        }
    }
}
```

### Siehe auch

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


