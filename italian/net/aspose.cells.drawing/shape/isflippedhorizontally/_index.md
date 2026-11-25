---
title: "Shape.IsFlippedHorizontally"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Ottiene e imposta se la forma è capovolta orizzontalmente"
type: docs
url: /it/net/aspose.cells.drawing/shape/isflippedhorizontally/
---
## Shape.IsFlippedHorizontally property

Ottiene e imposta se la forma è capovolta orizzontalmente.

```csharp
public bool IsFlippedHorizontally { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsFlippedHorizontallyDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma di esempio con tutti i parametri richiesti
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Verifica e capovolgi orizzontalmente se non è già capovolta
            if (shape.IsFlippedHorizontally == false)
            {
                shape.IsFlippedHorizontally = true;
                Console.WriteLine("Shape was flipped horizontally");
            }
            else
            {
                Console.WriteLine("Shape was already flipped horizontally");
            }
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


