---
title: "FillFormat.TextureFill"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FillFormat-Eigenschaft. Gibt das TextureFill-Objekt zurück"
type: docs
url: /de/net/aspose.cells.drawing/fillformat/texturefill/
---
## FillFormat.TextureFill property

Gibt das `TextureFill`-Objekt zurück.

```csharp
public TextureFill TextureFill { get; }
```

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyTextureFillDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie eine Bildform hinzu
            string imagePath = Path.Combine("your_image_directory", "texture.png");
            int pictureIndex = worksheet.Pictures.Add(0, 0, imagePath);
            Shape picture = worksheet.Shapes[pictureIndex];

            // Texture-Füllungseigenschaften festlegen
            picture.Fill.TextureFill.ImageData = File.ReadAllBytes(imagePath);
            picture.Fill.TextureFill.IsTiling = true;
            picture.Fill.TextureFill.Scale = 0.5;

            // Speichere die Arbeitsmappe
            workbook.Save("TextureFillDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TextureFill](../../texturefill/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


