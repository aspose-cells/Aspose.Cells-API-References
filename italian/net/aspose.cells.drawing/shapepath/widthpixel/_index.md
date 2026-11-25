---
title: "ShapePath.WidthPixel"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ShapePath proprietà. Ottiene la larghezza di questo percorso in unità di pixel"
type: docs
url: /it/net/aspose.cells.drawing/shapepath/widthpixel/
---
## ShapePath.WidthPixel property

Restituisce la larghezza di questo percorso in unità di pixel.

```csharp
public int WidthPixel { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPropertyWidthPixelDemo
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

                // Visualizza il valore iniziale di WidthPixel
                Console.WriteLine("Initial WidthPixel value: " + shapePath.WidthPixel);

                // Imposta un nuovo valore di larghezza
                shapePath.WidthPixel = 300;
                Console.WriteLine("Updated WidthPixel value: " + shapePath.WidthPixel);

                // Aggiungi la forma al foglio di lavoro
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, shapePath.WidthPixel, 200, new ShapePath[] { shapePath });

                // Salva la cartella di lavoro
                workbook.Save("WidthPixelDemo.xlsx");
                Console.WriteLine("WidthPixel property demonstrated successfully.");
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


