---
title: "Shape.IsLocked"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Sant betyder att objektet inte kan ändras när bladet är skyddat. Observera att detta värde bara är meningsfullt om kalkylbladet eller objekten i kalkylbladet är skyddade"
type: docs
url: /sv/net/aspose.cells.drawing/shape/islocked/
---
## Shape.IsLocked property

Sant betyder att objektet inte kan ändras när bladet är skyddat. Observera att detta värde endast är meningsfullt om arbetsbladet eller objekten i arbetsbladet är skyddade.

```csharp
public bool IsLocked { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsLockedDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form i kalkylbladet
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 100);

            // Skydda kalkylbladet
            worksheet.Protect(ProtectionType.All);

            // Demonstrera låsning/upplåsning av formen
            Console.WriteLine("Original IsLocked state: " + shape.IsLocked);

            // Lås upp formen
            shape.IsLocked = false;
            Console.WriteLine("After unlocking, IsLocked state: " + shape.IsLocked);

            // Lås formen
            shape.IsLocked = true;
            Console.WriteLine("After locking, IsLocked state: " + shape.IsLocked);
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


