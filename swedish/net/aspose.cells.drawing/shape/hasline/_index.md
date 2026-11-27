---
title: "Shape.HasLine"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Hämtar och anger om linjekanten på formen är synlig"
type: docs
url: /sv/net/aspose.cells.drawing/shape/hasline/
---
## Shape.HasLine property

Hämtar och anger om figurens linjekant är synlig.

```csharp
public bool HasLine { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHasLineDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en exempelform med alla nödvändiga parametrar
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            // Demonstrera HasLine-egenskapen
            Console.WriteLine("Shape initially has line: " + shape.HasLine);
            
            // Ta bort linjen
            shape.HasLine = false;
            Console.WriteLine("After setting HasLine to false: " + shape.HasLine);
            
            // Lägg till linjen igen
            shape.HasLine = true;
            Console.WriteLine("After setting HasLine to true: " + shape.HasLine);
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


