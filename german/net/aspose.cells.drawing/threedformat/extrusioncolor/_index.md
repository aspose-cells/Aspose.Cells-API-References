---
title: "ThreeDFormat.ExtrusionColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ThreeDFormat property. Gibt die Extrusionsfarbe einer Form zurück"
type: docs
url: /de/net/aspose.cells.drawing/threedformat/extrusioncolor/
---
## ThreeDFormat.ExtrusionColor property

Liest die Extrusionsfarbe einer Form.

```csharp
public CellsColor ExtrusionColor { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyExtrusionColorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Form hinzu, um die 3D-Formatierung zu demonstrieren.
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 1, 1, 0, 0, 200, 100);
            shape.Text = "3D ExtrusionColor Demo";
            
            // Hole das ThreeDFormat der Form.
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Grundlegende 3D‑Eigenschaften konfigurieren, um die Extrusion sichtbar zu machen
            threeDFormat.ExtrusionHeight = 20;
            threeDFormat.ContourWidth = 2;
            threeDFormat.Material = PresetMaterialType.Plastic;

            try
            {
                // Den Wert von ExtrusionColor abrufen und anzeigen
                CellsColor extrusionColor = threeDFormat.ExtrusionColor;
                Console.WriteLine("ExtrusionColor properties:");
                Console.WriteLine($"Type: {extrusionColor.Type}");
                Console.WriteLine($"Color (RGB): {extrusionColor.Color}");
                Console.WriteLine($"Transparency: {extrusionColor.Transparency}");

                // Arbeitsmappe speichern, um die 3D‑Effekte zu sehen
                workbook.Save("ThreeDFormatExtrusionColorDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


