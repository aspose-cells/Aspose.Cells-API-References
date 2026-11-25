---
title: "Enum FillPictureType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.FillPictureType enum. Rappresenta il tipo di riempimento immagine"
type: docs
url: /it/net/aspose.cells.drawing/fillpicturetype/
---
## FillPictureType enumeration

Rappresenta il tipo di riempimento immagine.

```csharp
public enum FillPictureType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Stretch | `0` | Allunga |
| Stack | `1` | Impila |
| StackAndScale | `2` | StackAndScale |

### Esempi

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

            // Aggiungi una forma rettangolare per dimostrare il riempimento immagine
            Shape shape = worksheet.Shapes.AddRectangle(2, 0, 2, 0, 200, 200);

            // Imposta le proprietà del riempimento immagine
            shape.Fill.Type = FillType.Texture;
            shape.Fill.PictureFormatType = FillPictureType.StackAndScale;

            // Usa un'immagine minimale di 1x1 pixel (bianca) per la dimostrazione
            string base64Image = "iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAQAAAC1HAwCAAAAC0lEQVR42mNkYAAAAAYAAjCB0C8AAAAASUVORK5CYII=";
            shape.Fill.ImageData = Convert.FromBase64String(base64Image);

            // Aggiungi un'altra forma con un tipo di riempimento diverso
            Shape shape2 = worksheet.Shapes.AddRectangle(2, 5, 2, 0, 200, 200);
            shape2.Fill.Type = FillType.Texture;
            shape2.Fill.PictureFormatType = FillPictureType.Stretch;
            shape2.Fill.ImageData = Convert.FromBase64String(base64Image);

            // Salva la cartella di lavoro con diverse configurazioni di riempimento
            workbook.Save("FillPictureTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


