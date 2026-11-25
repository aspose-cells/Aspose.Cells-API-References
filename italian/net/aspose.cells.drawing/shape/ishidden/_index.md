---
title: "Shape.IsHidden"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Indica se l'oggetto è visibile"
type: docs
url: /it/net/aspose.cells.drawing/shape/ishidden/
---
## Shape.IsHidden property

Indica se l'oggetto è visibile.

```csharp
public bool IsHidden { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsHiddenDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma al foglio di lavoro
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Imposta la proprietà IsHidden su false (visibile)
            shape.IsHidden = false;
            Console.WriteLine("Shape is visible: " + !shape.IsHidden);

            // Imposta la proprietà IsHidden su true (nascosto)
            shape.IsHidden = true;
            Console.WriteLine("Shape is hidden: " + shape.IsHidden);
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


