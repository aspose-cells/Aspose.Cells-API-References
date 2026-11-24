---
title: "Bevel.Width"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Bevel Eigenschaft. Gibt die Breite des Abschrägungsrands zurück und legt sie fest, bzw. wie weit in die Form er angewendet wird. In Einheit von Punkten"
type: docs
url: /de/net/aspose.cells.drawing/bevel/width/
---
## Bevel.Width property

Liest und setzt die Breite der Abschrägung bzw. wie weit in die Form sie angewendet wird. In Punkten.

```csharp
public double Width { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class BevelPropertyWidthDemo
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

            // Diagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 5, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Erste Serie abrufen und 3D-Format festlegen
            Series series = chart.NSeries[0];
            Format3D format3D = series.ShapeProperties.Format3D;
            
            // Bevel-Eigenschaften mit Width demonstrieren konfigurieren
            Bevel topBevel = format3D.TopBevel;
            topBevel.Type = BevelPresetType.Circle;
            topBevel.Width = 12; // Demonstrating Width property
            topBevel.Height = 6;

            // Speichere die Arbeitsmappe
            workbook.Save("BevelWidthDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Bevel](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


