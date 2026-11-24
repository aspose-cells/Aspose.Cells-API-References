---
title: "PicFormatOption.Right"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PicFormatOption-Eigenschaft. Liest oder schreibt den rechten Versatz zum Dehnen des Bildes"
type: docs
url: /de/net/aspose.cells.drawing/picformatoption/right/
---
## PicFormatOption.Right property

Liest oder legt den rechten Versatz für das Dehnen des Bildes fest.

```csharp
public double Right { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class PicFormatOptionPropertyRightDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe und greife auf das erste Arbeitsblatt zu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Rechteckform mit angegebenen Abmessungen hinzu
            Shape shape = worksheet.Shapes.AddRectangle(5, 2, 10, 10, 150, 300);

            // Konfiguriere die Bildfüllung für die Form
            shape.Fill.FillType = FillType.Texture;
            string imagePath = "sample.jpg"; // Replace with actual image path
            
            if (File.Exists(imagePath))
            {
                shape.Fill.ImageData = File.ReadAllBytes(imagePath);
            }
            else
            {
                Console.WriteLine("Image not found - using empty picture fill");
            }

            // Greife über TextureFill auf die Bildformatoptionen zu
            PicFormatOption picFormat = shape.Fill.TextureFill.PicFormatOption;

            // Zeige die Right-Eigenschaft an und ändere sie
            Console.WriteLine("Initial Right offset: " + picFormat.Right);
            picFormat.Right = 25.5; // Set right offset to 25.5 units

            // Überprüfe den neuen Wert und speichere die Änderungen
            Console.WriteLine("Updated Right offset: " + picFormat.Right);
            workbook.Save("RightPropertyDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


