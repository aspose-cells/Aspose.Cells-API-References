---
title: "Shape.TextVerticalOverflow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Ottiene e imposta il tipo di overflow verticale del testo della forma che contiene testo"
type: docs
url: /it/net/aspose.cells.drawing/shape/textverticaloverflow/
---
## Shape.TextVerticalOverflow property

Ottiene e imposta il tipo di overflow verticale del testo della forma che contiene testo.

```csharp
public TextOverflowType TextVerticalOverflow { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextVerticalOverflowDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 200, 100);
            
            // Imposta il testo e fallo traboccare verticalmente
            shape.Text = "This is a long text that will demonstrate vertical text overflow functionality in the shape.";
            shape.TextVerticalOverflow = TextOverflowType.Overflow;

            // Salva la cartella di lavoro
            workbook.Save("ShapeTextVerticalOverflowDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [TextOverflowType](../../textoverflowtype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


