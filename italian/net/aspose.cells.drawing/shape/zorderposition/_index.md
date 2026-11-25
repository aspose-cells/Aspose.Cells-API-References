---
title: "Shape.ZOrderPosition"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Restituisce la posizione di una forma nell'ordine Z"
type: docs
url: /it/net/aspose.cells.drawing/shape/zorderposition/
---
## Shape.ZOrderPosition property

Restituisce la posizione di una shape nell'ordine Z.

```csharp
public int ZOrderPosition { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyZOrderPositionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi tre forme per dimostrare ZOrder
            Shape shape1 = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);
            Shape shape2 = worksheet.Shapes.AddRectangle(50, 50, 100, 100, 0, 0);
            Shape shape3 = worksheet.Shapes.AddRectangle(90, 90, 100, 100, 0, 0);

            // Imposta le posizioni ZOrder
            shape1.ZOrderPosition = 0;
            shape2.ZOrderPosition = 1;
            shape3.ZOrderPosition = 2;

            // Cambia ZOrder di shape3 per portarla in primo piano
            shape3.ZOrderPosition = 0;

            // Salva la cartella di lavoro
            workbook.Save("ShapeZOrderDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


