---
title: "ShapePath.HeightPixel"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ShapePath proprietà. Ottiene l'altezza di questo percorso in unità di pixel"
type: docs
url: /it/net/aspose.cells.drawing/shapepath/heightpixel/
---
## ShapePath.HeightPixel property

Restituisce l'altezza di questo percorso in unità di pixel.

```csharp
public int HeightPixel { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPropertyHeightPixelDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Crea un nuovo percorso di forma
                ShapePath shapePath = new ShapePath();

                // Crea un percorso rettangolare semplice
                shapePath.MoveTo(10, 10);
                shapePath.LineTo(100, 10);
                shapePath.LineTo(100, 50);
                shapePath.LineTo(10, 50);
                shapePath.Close();

                // Visualizza il valore corrente di HeightPixel
                Console.WriteLine("Initial HeightPixel value: " + shapePath.HeightPixel);

                // Imposta un nuovo valore di altezza
                shapePath.HeightPixel = 200;
                Console.WriteLine("Updated HeightPixel value: " + shapePath.HeightPixel);

                // Aggiungi la forma al foglio di lavoro
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath });

                // Salva la cartella di lavoro
                workbook.Save("HeightPixelDemo.xlsx");
                Console.WriteLine("HeightPixel property demonstrated successfully.");
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

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


