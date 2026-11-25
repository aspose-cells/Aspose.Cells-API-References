---
title: "TextureFill.Transparency"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextureFill. Restituisce o imposta il grado di trasparenza dell'area come valore da 0,0 opaco a 1,0 chiaro"
type: docs
url: /it/net/aspose.cells.drawing/texturefill/transparency/
---
## TextureFill.Transparency property

Restituisce o imposta il grado di trasparenza dell'area come valore da 0,0 (opaco) a 1,0 (trasparente).

```csharp
public double Transparency { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class TextureFillPropertyTransparencyDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare al foglio di lavoro
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 200);

            // Imposta il tipo di riempimento a texture
            shape.Fill.FillType = FillType.Texture;

            // Accedi alle proprietà di riempimento texture
            TextureFill textureFill = shape.Fill.TextureFill;

            // Imposta un tipo di texture incorporato
            textureFill.Type = TextureType.BlueTissuePaper;

            // Visualizza il valore iniziale di trasparenza
            Console.WriteLine("Initial Transparency: " + textureFill.Transparency);

            // Modifica la trasparenza al 70% (0,0 = opaco, 1,0 = completamente trasparente)
            textureFill.Transparency = 0.7;
            Console.WriteLine("Updated Transparency: " + textureFill.Transparency);

            // Salva la cartella di lavoro con effetto di trasparenza visibile
            workbook.Save("TextureFillTransparencyDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


