---
title: "Shape.WidthInShape"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Rappresenta la larghezza della forma in unità di 1/4000 della forma genitore"
type: docs
url: /it/net/aspose.cells.drawing/shape/widthinshape/
---
## Shape.WidthInShape property

Rappresenta la larghezza della forma, in unità di 1/4000 della forma padre.

```csharp
public int WidthInShape { get; set; }
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
    public class ShapePropertyWidthInShapeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea due forme rettangolari
            Shape rect1 = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 100);
            Shape rect2 = worksheet.Shapes.AddRectangle(0, 100, 0, 0, 100, 100);
            
            // Raggruppa le forme utilizzando oggetti shape
            GroupShape group = worksheet.Shapes.Group(new Shape[] { rect1, rect2 });
            
            // Dimostra l'uso di WidthInShape
            if (rect1.IsInGroup && rect1.WidthInShape == 2000)
            {
                rect1.WidthInShape = 4000;
            }
            
            // Salvare la cartella di lavoro modificata
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


