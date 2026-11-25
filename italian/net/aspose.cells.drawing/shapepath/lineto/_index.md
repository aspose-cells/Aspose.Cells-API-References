---
title: "ShapePath.LineTo"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ShapePath. Aggiunge un segmento di linea alla figura corrente. Il punto di partenza è il punto finale della figura corrente. Unità Pixel"
type: docs
url: /it/net/aspose.cells.drawing/shapepath/lineto/
---
## ShapePath.LineTo method

Aggiunge un segmento di linea alla figura corrente. Il punto di partenza è il punto finale della figura corrente. Unità: Pixel.

```csharp
public void LineTo(float x, float y)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| x | Single | La coordinata x del punto finale del segmento di linea (Unità: Pixel). |
| y | Single | La coordinata y del punto finale del segmento di linea (Unità: Pixel). |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodLineToWithSingleSingleDemo
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

                Console.WriteLine("LineTo method executed successfully with parameters (Single, Single)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing LineTo method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("ShapePathMethodLineToWithSingleSingleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


