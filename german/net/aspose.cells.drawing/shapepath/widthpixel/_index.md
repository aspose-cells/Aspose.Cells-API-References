---
title: "ShapePath.WidthPixel"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapePath-Eigenschaft. Gibt die Breite dieses Pfads in Pixeln zurück"
type: docs
url: /de/net/aspose.cells.drawing/shapepath/widthpixel/
---
## ShapePath.WidthPixel property

Ermittelt die Breite dieses Pfads in Pixeln.

```csharp
public int WidthPixel { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPropertyWidthPixelDemo
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

                // Zeige den initialen WidthPixel-Wert an
                Console.WriteLine("Initial WidthPixel value: " + shapePath.WidthPixel);

                // Setze einen neuen Breitenwert
                shapePath.WidthPixel = 300;
                Console.WriteLine("Updated WidthPixel value: " + shapePath.WidthPixel);

                // Füge die Form dem Arbeitsblatt hinzu
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, shapePath.WidthPixel, 200, new ShapePath[] { shapePath });

                // Speichere die Arbeitsmappe
                workbook.Save("WidthPixelDemo.xlsx");
                Console.WriteLine("WidthPixel property demonstrated successfully.");
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


