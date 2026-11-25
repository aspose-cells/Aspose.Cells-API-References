---
title: "CellsColor.SetTintOfShapeColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo CellsColor. Imposta la tinta del colore della forma"
type: docs
url: /it/net/aspose.cells/cellscolor/settintofshapecolor/
---
## CellsColor.SetTintOfShapeColor method

Imposta la tinta del colore della forma

```csharp
public void SetTintOfShapeColor(double tint)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| tinta | Double |  |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class CellsColorMethodSetTintOfShapeColorWithDoubleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma al foglio di lavoro
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            try
            {
                // Ottieni il colore di riempimento della forma
                CellsColor shapeColor = shape.Fill.SolidFill.CellsColor;
                
                // Imposta il colore da trattare come colore della forma
                shapeColor.IsShapeColor = true;
                
                // Imposta la tinta del colore della forma (intervallo valido è da -1.0 a 1.0)
                shapeColor.SetTintOfShapeColor(0.5); // Lighten the color by 50%
                
                Console.WriteLine("SetTintOfShapeColor method executed successfully with parameter 0.5");
                
                // Visualizza l'effetto modificando il colore di riempimento della forma
                shape.Fill.SolidFill.Color = System.Drawing.Color.Blue;
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTintOfShapeColor method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("SetTintOfShapeColorWithDoubleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


