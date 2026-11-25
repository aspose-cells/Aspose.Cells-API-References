---
title: "TextureFill.Scale"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextureFill. Ottiene e imposta la scala del formato immagine"
type: docs
url: /it/net/aspose.cells.drawing/texturefill/scale/
---
## TextureFill.Scale property

Ottiene e imposta la scala del formato immagine.

```csharp
public double Scale { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class TextureFillPropertyScaleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma e ottieni il suo formato di riempimento
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 10, 10, 500, 300);
            FillFormat fillFormat = shape.Fill;

            // Configura il riempimento texture
            fillFormat.FillType = FillType.Texture;
            TextureFill textureFill = fillFormat.TextureFill;

            // Carica l'immagine texture e configura le proprietà
            textureFill.ImageData = File.ReadAllBytes("texture.jpg");
            textureFill.Type = TextureType.Unknown; // Changed from UserDefined to Unknown
            textureFill.IsTiling = true;

            // Visualizza e modifica la scala
            Console.WriteLine("Initial Scale: " + textureFill.Scale);
            textureFill.Scale = 0.5;
            Console.WriteLine("Modified Scale: " + textureFill.Scale);

            // Salva il risultato
            workbook.Save("TextureFillScaleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


