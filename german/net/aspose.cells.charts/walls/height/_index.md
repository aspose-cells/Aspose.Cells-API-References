---
title: "Walls.Height"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Walls-Eigenschaft. Gibt die Höhe von oben nach unten in Einheiten von 1/4000 der Diagrammhöhe zurück, nachdem die Methode Chart.Calculate aufgerufen wurde."
type: docs
url: /de/net/aspose.cells.charts/walls/height/
---
## Walls.Height property

Liest die Höhe von oben nach unten in Einheiten von 1/4000 der Diagrammhöhe nach Aufruf der Methode Chart.Calculate().

```csharp
public int Height { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class WallsPropertyHeightDemo
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

            // Greifen Sie auf walls zu und demonstrieren Sie die Height‑Eigenschaft
            Walls walls = chart.Walls;
            Console.WriteLine("Wall Height: " + walls.Height);
            Console.WriteLine("Wall Height in Pixels: " + walls.HeightPx);

            // Ändern Sie die Diagrammbereichsgröße anstelle der direkten Height‑Eigenschaft
            chart.ChartObject.Height = 400;
            chart.Calculate();
            Console.WriteLine("After resizing - Wall Height: " + walls.Height);
            Console.WriteLine("After resizing - Wall Height in Pixels: " + walls.HeightPx);

            workbook.Save("WallsHeightDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


