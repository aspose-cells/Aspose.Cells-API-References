---
title: "PicFormatOption.Right"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PicFormatOption. Ottiene o imposta l'offset destro per l'allungamento dell'immagine"
type: docs
url: /it/net/aspose.cells.drawing/picformatoption/right/
---
## PicFormatOption.Right property

Ottiene o imposta lo spostamento destro per lo stretching dell'immagine.

```csharp
public double Right { get; set; }
```

### Esempi

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
            // Crea una nuova cartella di lavoro e accedi al primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare con dimensioni specificate
            Shape shape = worksheet.Shapes.AddRectangle(5, 2, 10, 10, 150, 300);

            // Configura il riempimento dell'immagine per la forma
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

            // Accedi alle opzioni di formato immagine tramite TextureFill
            PicFormatOption picFormat = shape.Fill.TextureFill.PicFormatOption;

            // Visualizza e modifica la proprietà Right
            Console.WriteLine("Initial Right offset: " + picFormat.Right);
            picFormat.Right = 25.5; // Set right offset to 25.5 units

            // Verifica il nuovo valore e salva le modifiche
            Console.WriteLine("Updated Right offset: " + picFormat.Right);
            workbook.Save("RightPropertyDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


