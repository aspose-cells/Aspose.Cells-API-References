---
title: "FillFormat.TextureFill"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FillFormat. Ottiene l'oggetto TextureFill"
type: docs
url: /it/net/aspose.cells.drawing/fillformat/texturefill/
---
## FillFormat.TextureFill property

Ottiene l'oggetto `TextureFill`.

```csharp
public TextureFill TextureFill { get; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma immagine
            string imagePath = Path.Combine("your_image_directory", "texture.png");
            int pictureIndex = worksheet.Pictures.Add(0, 0, imagePath);
            Shape picture = worksheet.Shapes[pictureIndex];

            // Imposta le proprietà del riempimento texture
            picture.Fill.TextureFill.ImageData = File.ReadAllBytes(imagePath);
            picture.Fill.TextureFill.IsTiling = true;
            picture.Fill.TextureFill.Scale = 0.5;

            // Salva la cartella di lavoro
            workbook.Save("TextureFillDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TextureFill](../../texturefill/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


