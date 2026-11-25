---
title: "Shape.TextVerticalAlignment"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Ottiene e imposta il tipo di allineamento verticale del testo della forma"
type: docs
url: /it/net/aspose.cells.drawing/shape/textverticalalignment/
---
## Shape.TextVerticalAlignment property

Ottiene e imposta il tipo di allineamento verticale del testo della forma.

```csharp
public TextAlignmentType TextVerticalAlignment { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextVerticalAlignmentDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // Imposta il testo e l'allineamento
            shape.Text = "Vertical Alignment Demo";
            shape.TextVerticalAlignment = TextAlignmentType.Bottom;
            
            Console.WriteLine("Initial Vertical Alignment: " + shape.TextVerticalAlignment);

            // Cambia l'allineamento verticale
            if (shape.TextVerticalAlignment == TextAlignmentType.Bottom)
            {
                shape.TextVerticalAlignment = TextAlignmentType.Center;
            }

            Console.WriteLine("Updated Vertical Alignment: " + shape.TextVerticalAlignment);

            // Salva la cartella di lavoro
            workbook.Save("TextVerticalAlignmentDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


