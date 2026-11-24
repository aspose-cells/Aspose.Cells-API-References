---
title: "SolidFill.Transparency"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SolidFill-Eigenschaft. Gibt den Transparenzgrad des Bereichs zurück oder legt ihn fest, als Wert von 0.0 (undurchsichtig) bis 1.0 (klar)."
type: docs
url: /de/net/aspose.cells.drawing/solidfill/transparency/
---
## SolidFill.Transparency property

Gibt den Transparenzgrad des Bereichs zurück oder legt ihn fest, als Wert von 0,0 (undurchsichtig) bis 1,0 (transparent).

```csharp
public double Transparency { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SolidFillPropertyTransparencyDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Beispieldaten für das Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            chart.Calculate();

            // Füge eine Form hinzu, um Transparenz zu demonstrieren
            Shape shape = chart.Shapes.AddShapeInChart(MsoDrawingType.Rectangle, PlacementType.FreeFloating, 
                1000, 1000, 2000, 2000);
            
            // Setzen Sie eine einfarbige Füllung mit Transparenz.
            shape.Fill.SolidFill.Color = Color.Blue;
            shape.Fill.SolidFill.Transparency = 0.5; // 50% transparent

            // Fügen Sie ein weiteres Shape zum Vergleich hinzu (vollständig undurchsichtig).
            Shape shape2 = chart.Shapes.AddShapeInChart(MsoDrawingType.Rectangle, PlacementType.FreeFloating, 
                3000, 1000, 2000, 2000);
            shape2.Fill.SolidFill.Color = Color.Blue;
            shape2.Fill.SolidFill.Transparency = 0; // 0% transparent (fully opaque)

            // Speichere die Arbeitsmappe
            workbook.Save("SolidFillTransparencyDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SolidFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


