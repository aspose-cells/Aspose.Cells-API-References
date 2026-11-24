---
title: "Enum FillPictureType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.FillPictureType Enum. Stellt den Bildfülltyp dar"
type: docs
url: /de/net/aspose.cells.drawing/fillpicturetype/
---
## FillPictureType enumeration

Stellt den Bildfülltyp dar.

```csharp
public enum FillPictureType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Stretch | `0` | Strecken |
| Stack | `1` | Stapel |
| StackAndScale | `2` | StackAndScale |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassFillPictureTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie eine Rechteckform hinzu, um die Bildfüllung zu demonstrieren
            Shape shape = worksheet.Shapes.AddRectangle(2, 0, 2, 0, 200, 200);

            // Legen Sie die Eigenschaften der Bildfüllung fest
            shape.Fill.Type = FillType.Texture;
            shape.Fill.PictureFormatType = FillPictureType.StackAndScale;

            // Verwenden Sie ein minimales 1x1-Pixel-Bild (weiß) für die Demonstration
            string base64Image = "iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAQAAAC1HAwCAAAAC0lEQVR42mNkYAAAAAYAAjCB0C8AAAAASUVORK5CYII=";
            shape.Fill.ImageData = Convert.FromBase64String(base64Image);

            // Fügen Sie eine weitere Form mit anderem Fülltyp hinzu
            Shape shape2 = worksheet.Shapes.AddRectangle(2, 5, 2, 0, 200, 200);
            shape2.Fill.Type = FillType.Texture;
            shape2.Fill.PictureFormatType = FillPictureType.Stretch;
            shape2.Fill.ImageData = Convert.FromBase64String(base64Image);

            // Speichern Sie die Arbeitsmappe mit verschiedenen Füllkonfigurationen
            workbook.Save("FillPictureTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


