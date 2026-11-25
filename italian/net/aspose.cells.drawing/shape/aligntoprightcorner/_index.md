---
title: "Shape.AlignTopRightCorner"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Shape. Sposta l'immagine nell'angolo in alto a destra"
type: docs
url: /it/net/aspose.cells.drawing/shape/aligntoprightcorner/
---
## Shape.AlignTopRightCorner method

Sposta l'immagine nell'angolo in alto a destra.

```csharp
public void AlignTopRightCorner(int topRow, int rightColumn)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | Int32 | l'indice della riga. |
| rightColumn | Int32 | l'indice della colonna. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodAlignTopRightCornerWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma di esempio da allineare
            Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);

            // Allinea l'angolo in alto a destra della forma alla riga 2, colonna 5
            shape.AlignTopRightCorner(2, 5);

            // Salva la cartella di lavoro
            workbook.Save("AlignTopRightCornerDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


