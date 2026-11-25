---
title: "Shape.AnchorType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Ottiene e imposta il tipo del segnaposto di ancoraggio della forma."
type: docs
url: /it/net/aspose.cells.drawing/shape/anchortype/
---
## Shape.AnchorType property

Ottiene e imposta il tipo del segnaposto di ancoraggio della forma.

```csharp
public ShapeAnchorType AnchorType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyAnchorTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma con tipo di ancoraggio predefinito.
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 0, 0);
            
            // Verifica e modifica il tipo di ancoraggio.
            if (shape.AnchorType == ShapeAnchorType.OneCellAnchor)
            {
                shape.AnchorType = ShapeAnchorType.TwoCellAnchor;
                Console.WriteLine("Anchor type changed to TwoCellAnchor");
            }
            
            // Salva la cartella di lavoro
            workbook.Save("ShapeAnchorTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ShapeAnchorType](../../shapeanchortype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


