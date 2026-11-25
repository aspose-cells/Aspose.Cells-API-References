---
title: "Shape.UpperLeftColumn"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Rappresenta l'indice della colonna dell'angolo in alto a sinistra"
type: docs
url: /it/net/aspose.cells.drawing/shape/upperleftcolumn/
---
## Shape.UpperLeftColumn property

Rappresenta l'indice della colonna dell'angolo in alto a sinistra.

```csharp
public int UpperLeftColumn { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyUpperLeftColumnDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma al foglio di lavoro con tutti i parametri richiesti
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 100, 100, 100);

            // Imposta e dimostra la proprietà UpperLeftColumn
            shape.UpperLeftColumn = 3;
            Console.WriteLine("Shape's initial leftColumn: " + shape.UpperLeftColumn);

            // Modifica l'UpperLeftColumn
            if (shape.UpperLeftColumn == 3)
            {
                shape.UpperLeftColumn = 1;
                Console.WriteLine("Shape's modified leftColumn: " + shape.UpperLeftColumn);
            }

            // Salva la cartella di lavoro
            workbook.Save("ShapeUpperLeftColumnDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


