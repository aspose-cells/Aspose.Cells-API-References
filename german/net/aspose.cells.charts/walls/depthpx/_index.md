---
title: "Walls.DepthPx"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Walls-Eigenschaft. Gibt die Tiefe von vorne nach hinten in Pixeln zurück, nachdem die Methode Chart.Calculate aufgerufen wurde."
type: docs
url: /de/net/aspose.cells.charts/walls/depthpx/
---
## Walls.DepthPx property

Liest die Tiefe von vorne nach hinten in Pixeln nach Aufruf der Methode Chart.Calculate().

```csharp
public int DepthPx { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class WallsPropertyDepthPxDemo
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

            // Erstellen Sie ein 3D-Diagramm
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Rufen Sie walls ab und demonstrieren Sie die DepthPx‑Eigenschaft
            Walls walls = chart.Walls;
            Console.WriteLine("Wall Depth in Pixels: " + walls.DepthPx);

            // Arbeitsmappe speichern.
            workbook.Save("WallsDepthPxDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


