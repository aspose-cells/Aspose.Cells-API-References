---
title: "Axis.MinorUnit"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Axis-Eigenschaft. Stellt die Nebeneinheiten für die Achse dar"
type: docs
url: /de/net/aspose.cells.charts/axis/minorunit/
---
## Axis.MinorUnit property

Gibt die Nebeneinheiten für die Achse an.

```csharp
public double MinorUnit { get; set; }
```

### Hinweise

Die Nebeneinheiten müssen größer als Null sein.

### Beispiele

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyMinorUnitDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // Fügen Sie Beispieldaten hinzu
            cells["A1"].PutValue("Region");
            cells["A2"].PutValue("France");
            cells["A3"].PutValue("Germany");
            cells["A4"].PutValue("England");
            cells["B1"].PutValue("Sales");
            cells["B2"].PutValue(70000);
            cells["B3"].PutValue(55000);
            cells["B4"].PutValue(30000);

            // Diagramm erstellen
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 1, 20, 10);
            Chart chart = sheet.Charts[chartIndex];

            // Diagrammdaten konfigurieren
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Werteachse konfigurieren
            chart.ValueAxis.Title.Text = "Sales Amount";
            chart.ValueAxis.MajorUnit = 20000;
            chart.ValueAxis.MinorUnit = 5000; // Demonstrate MinorUnit property
            chart.ValueAxis.MinValue = 0;
            chart.ValueAxis.MaxValue = 80000;

            // Speichere die Arbeitsmappe
            workbook.Save("AxisPropertyMinorUnitDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


