---
title: "Chart.Walls"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Chart-Eigenschaft. Gibt ein Walls-Objekt zurück, das die Wände eines 3D-Diagramms darstellt"
type: docs
url: /de/net/aspose.cells.charts/chart/walls/
---
## Chart.Walls property

Gibt ein `Walls` Objekt zurück, das die Wände eines 3‑D‑Diagramms darstellt.

```csharp
public Walls Walls { get; }
```

### Hinweise

Diese Eigenschaft gilt nicht für 3‑D‑Kuchendiagramme.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPropertyWallsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(35);

            // Zylindrisches Säulendiagramm erstellen
            int chartIndex = worksheet.Charts.Add(ChartType.Cylinder, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammgrundlagen konfigurieren
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            chart.IsRectangularCornered = true;
            chart.RotationAngle = 20;

            // Wandeigenschaften konfigurieren
            Walls walls = chart.Walls;
            walls.BackgroundColor = Color.LightGray;
            walls.ForegroundColor = Color.Transparent;
            walls.FillFormat.SetPresetColorGradient(GradientPresetType.CalmWater, GradientStyleType.Horizontal, 1);

            // Ergebnis speichern
            workbook.Save("ChartWallsDemo_out.xlsx");
        }
    }
}
```

### Siehe auch

* class [Walls](../../walls/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


