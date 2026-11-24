---
title: "ThreeDFormat.ContourColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ThreeDFormat-Eigenschaft. Gibt die Konturfarbe einer Form zurück oder legt sie fest."
type: docs
url: /de/net/aspose.cells.drawing/threedformat/contourcolor/
---
## ThreeDFormat.ContourColor property

Liest und setzt die Konturfarbe einer Form.

```csharp
public CellsColor ContourColor { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyContourColorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Form hinzu, um die 3D-Formatierung zu demonstrieren.
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 1, 1, 200, 100, 0, 0);
            shape.Text = "3D ContourColor Demo";
            
            // Hole das ThreeDFormat der Form.
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Konfiguriere grundlegende 3D-Eigenschaften.
            threeDFormat.TopBevelType = BevelType.ArtDeco;
            threeDFormat.TopBevelWidth = 10;
            threeDFormat.TopBevelHeight = 10;
            threeDFormat.ContourWidth = 2;

            try
            {
                // Hole den aktuellen ContourColor-Wert.
                CellsColor contourColor = threeDFormat.ContourColor;
                Console.WriteLine($"Initial ContourColor - Type: {contourColor.Type}, ARGB: {contourColor.Argb}");

                // Erstelle eine neue Farbe, indem du die bestehende änderst.
                contourColor.Argb = System.Drawing.Color.Red.ToArgb();
                contourColor.Transparency = 0.5;
                threeDFormat.ContourColor = contourColor;

                // Zeige den neuen ContourColor-Wert an.
                Console.WriteLine($"New ContourColor - Type: {threeDFormat.ContourColor.Type}, ARGB: {threeDFormat.ContourColor.Argb}");

                // Speichere die Arbeitsmappe, um die Auswirkungen zu sehen
                workbook.Save("ThreeDFormatContourColorDemo.xlsx");
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


