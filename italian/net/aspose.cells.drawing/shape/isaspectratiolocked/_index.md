---
title: "Shape.IsAspectRatioLocked"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. True indica che il rapporto d'aspetto della forma è bloccato"
type: docs
url: /it/net/aspose.cells.drawing/shape/isaspectratiolocked/
---
## Shape.IsAspectRatioLocked property

True indica che il rapporto d'aspetto della forma è bloccato.

```csharp
public bool IsAspectRatioLocked { get; set; }
```

### Osservazioni

Solo per immagini e oggetti Ole.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsAspectRatioLockedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 50);
            
            Console.WriteLine("Original Aspect Ratio Locked: " + shape.IsAspectRatioLocked);
            
            shape.IsAspectRatioLocked = true;
            Console.WriteLine("After setting to true: " + shape.IsAspectRatioLocked);
            
            shape.IsAspectRatioLocked = false;
            Console.WriteLine("After setting to false: " + shape.IsAspectRatioLocked);
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


