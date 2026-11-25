---
title: "ShapePath.MoveTo"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ShapePath metodo. Avvia una nuova figura dal punto specificato senza chiudere la figura corrente. Tutti i punti successivi aggiunti al percorso sono aggiunti a questa nuova figura. Unità Pixel"
type: docs
url: /it/net/aspose.cells.drawing/shapepath/moveto/
---
## ShapePath.MoveTo method

Avvia una nuova figura dal punto specificato senza chiudere la figura corrente. Tutti i punti successivi aggiunti al percorso vengono aggiati a questa nuova figura. Unità: Pixel.

```csharp
public void MoveTo(float x, float y)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| x | Single | La coordinata x del punto di partenza della figura (Unità: Pixel). |
| y | Single | La coordinata y del punto di partenza della figura (Unità: Pixel). |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodMoveToWithSingleSingleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                //Crea un nuovo percorso di forma
                ShapePath shapePath = new ShapePath();

                // Sposta al punto di partenza
                shapePath.MoveTo(10, 10);

                // Chiama il metodo LineTo con parametri (Single, Single)
                shapePath.LineTo(50.5f, 10.5f);
                shapePath.LineTo(50.5f, 50.5f);
                shapePath.LineTo(10.5f, 50.5f);
                shapePath.Close();

                //aggiungi forma libera
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath });

                Console.WriteLine("MoveTo method executed successfully with parameters (Single, Single)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing LineTo method: {ex.Message}");
            }
           
            
            // Salva il risultato
            workbook.Save("ShapePathMethodMoveToWithSingleSingleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


