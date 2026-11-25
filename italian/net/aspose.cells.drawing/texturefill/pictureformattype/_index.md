---
title: "TextureFill.PictureFormatType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextureFill. Ottiene e imposta il tipo di formato immagine"
type: docs
url: /it/net/aspose.cells.drawing/texturefill/pictureformattype/
---
## TextureFill.PictureFormatType property

Ottiene e imposta il tipo di formato immagine.

```csharp
public FillPictureType PictureFormatType { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class TextureFillPropertyPictureFormatTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare con tutti i parametri richiesti
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 200);

            // Imposta il tipo di riempimento a texture
            shape.Fill.FillType = FillType.Texture;
            TextureFill textureFill = shape.Fill.TextureFill;

            // Carica un'immagine PNG minima 1x1 pixel (bianca)
            string base64Image = "iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAQAAAC1HAwCAAAAC0lEQVR42mNkYAAAAAYAAjCB0C8AAAAASUVORK5CYII=";
            textureFill.ImageData = Convert.FromBase64String(base64Image);

            // Visualizza il PictureFormatType corrente
            Console.WriteLine("Initial PictureFormatType: " + textureFill.PictureFormatType);

            // Passa al formato impilato e abilita il tiling
            textureFill.PictureFormatType = FillPictureType.Stack;
            textureFill.IsTiling = true;

            // Aggiungi un'altra forma per confrontare il formato originale allungato
            Shape shape2 = worksheet.Shapes.AddRectangle(0, 0, 210, 0, 100, 200);
            shape2.Fill.FillType = FillType.Texture;
            TextureFill textureFill2 = shape2.Fill.TextureFill;
            textureFill2.ImageData = Convert.FromBase64String(base64Image);

            // Salva la cartella di lavoro con entrambi gli esempi di riempimento texture
            workbook.Save("TextureFillPictureFormatTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [FillPictureType](../../fillpicturetype/)
* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


