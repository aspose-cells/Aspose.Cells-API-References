---
title: "TextureFill.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextureFill. Ottiene e imposta il tipo di texture"
type: docs
url: /it/net/aspose.cells.drawing/texturefill/type/
---
## TextureFill.Type property

Ottiene e imposta il tipo di trama

```csharp
public TextureType Type { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class TextureFillPropertyTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare per dimostrare il riempimento a trama
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 200);

            // Imposta il tipo di riempimento a texture
            shape.Fill.FillType = FillType.Texture;

            // Accedi alle proprietà di riempimento texture
            TextureFill textureFill = shape.Fill.TextureFill;

            try
            {
                // Visualizza il valore iniziale di Type
                Console.WriteLine("Initial Texture Type: " + textureFill.Type);

                // Imposta un tipo di texture diverso
                textureFill.Type = TextureType.Granite;
                Console.WriteLine("Updated Texture Type: " + textureFill.Type);

                // Dimostra un altro tipo di texture
                textureFill.Type = TextureType.WaterDroplets;
                Console.WriteLine("Final Texture Type: " + textureFill.Type);

                // Salva la cartella di lavoro per vedere l'effetto
                workbook.Save("TextureFillTypeDemo.xlsx");
                Console.WriteLine("Texture fill type demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* enum [TextureType](../../texturetype/)
* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


