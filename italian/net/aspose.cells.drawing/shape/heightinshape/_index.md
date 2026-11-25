---
title: "Shape.HeightInShape"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Rappresenta lo spostamento verticale della forma dal bordo superiore della forma genitore in unità di 1/4000 dell'altezza della forma genitore"
type: docs
url: /it/net/aspose.cells.drawing/shape/heightinshape/
---
## Shape.HeightInShape property

Rappresenta lo spostamento verticale della forma dal bordo superiore della forma genitore, in unità di 1/4000 dell'altezza della forma genitore.

```csharp
public int HeightInShape { get; set; }
```

### Osservazioni

Si applica solo quando questa forma è nel gruppo o nel grafico.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHeightInShapeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi prima le forme con tutti i parametri richiesti
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 10, 10);
            Shape oval = worksheet.Shapes.AddOval(0, 0, 100, 100, 10, 120);

            // Raggruppa le forme
            Shape[] shapes = { rectangle, oval };
            GroupShape groupShape = worksheet.Shapes.Group(shapes);

            // Imposta l'altezza del rettangolo relativa alla forma di gruppo padre (1/4000 dell'altezza del padre)
            rectangle.HeightInShape = 2000; // Half the height of the parent
            oval.HeightInShape = 4000; // Full height of the parent

            // Salva la cartella di lavoro
            workbook.Save("ShapeHeightInShapeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


