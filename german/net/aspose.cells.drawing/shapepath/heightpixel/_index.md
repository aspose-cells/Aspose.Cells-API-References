---
title: "ShapePath.HeightPixel"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapePath-Eigenschaft. Gibt die Höhe dieses Pfads in Pixeln zurück"
type: docs
url: /de/net/aspose.cells.drawing/shapepath/heightpixel/
---
## ShapePath.HeightPixel property

Liefert die Höhe dieses Pfads in Pixeln.

```csharp
public int HeightPixel { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPropertyHeightPixelDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Erstellen Sie einen neuen Formpfad
                ShapePath shapePath = new ShapePath();

                // Erstelle einen einfachen Rechteckpfad
                shapePath.MoveTo(10, 10);
                shapePath.LineTo(100, 10);
                shapePath.LineTo(100, 50);
                shapePath.LineTo(10, 50);
                shapePath.Close();

                // Zeige den aktuellen HeightPixel-Wert an
                Console.WriteLine("Initial HeightPixel value: " + shapePath.HeightPixel);

                // Setze einen neuen Höhenwert
                shapePath.HeightPixel = 200;
                Console.WriteLine("Updated HeightPixel value: " + shapePath.HeightPixel);

                // Füge die Form dem Arbeitsblatt hinzu
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath });

                // Speichere die Arbeitsmappe
                workbook.Save("HeightPixelDemo.xlsx");
                Console.WriteLine("HeightPixel property demonstrated successfully.");
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

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


