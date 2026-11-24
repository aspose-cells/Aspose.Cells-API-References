---
title: "Walls.WidthPx"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Walls‑Eigenschaft. Gibt die Breite von links nach rechts in Pixeln zurück, nachdem die Chart.Calculate‑Methode aufgerufen wurde."
type: docs
url: /de/net/aspose.cells.charts/walls/widthpx/
---
## Walls.WidthPx property

Liest die Breite von links nach rechts in Pixeln nach Aufruf der Methode Chart.Calculate().

```csharp
public int WidthPx { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class WallsPropertyWidthPxDemo
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

            // Füge ein 3D‑Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            chart.Calculate();

            // Hole Walls und demonstriere die WidthPx‑Eigenschaft
            Walls walls = chart.Walls;
            Console.WriteLine("Wall width in pixels: " + walls.WidthPx);

            // Arbeitsmappe speichern.
            workbook.Save("WallsWidthPxDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


