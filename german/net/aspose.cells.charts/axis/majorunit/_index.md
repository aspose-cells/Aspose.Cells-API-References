---
title: "Axis.MajorUnit"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Axis-Eigenschaft. Gibt die Haupteinheiten für die Achse an"
type: docs
url: /de/net/aspose.cells.charts/axis/majorunit/
---
## Axis.MajorUnit property

Gibt die Haupteinheiten für die Achse an.

```csharp
public double MajorUnit { get; set; }
```

### Hinweise

Die Haupteinheiten müssen größer als Null sein.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyMajorUnitDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Category");
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue("Cat " + i);
                worksheet.Cells["B" + (i + 1)].PutValue(i * 10);
            }

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B11", true);
            chart.NSeries.CategoryData = "A2:A11";

            // Abrufen der Kategorienachse
            Axis axis = chart.CategoryAxis;

            // Anzeige der anfänglichen Haupteinheit
            Console.WriteLine("Initial Major Unit: " + axis.MajorUnit);

            // Neue Haupteinheit festlegen
            axis.MajorUnit = 3;
            Console.WriteLine("Modified Major Unit: " + axis.MajorUnit);

            // Speichere die Arbeitsmappe
            workbook.Save("AxisMajorUnitDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


