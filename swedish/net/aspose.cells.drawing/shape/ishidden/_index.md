---
title: "Shape.IsHidden"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Anger om objektet är synligt"
type: docs
url: /sv/net/aspose.cells.drawing/shape/ishidden/
---
## Shape.IsHidden property

Anger om objektet är synligt.

```csharp
public bool IsHidden { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form i kalkylbladet
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Ställ in IsHidden-egenskapen till false (synlig)
            shape.IsHidden = false;
            Console.WriteLine("Shape is visible: " + !shape.IsHidden);

            // Ställ in IsHidden-egenskapen till true (dold)
            shape.IsHidden = true;
            Console.WriteLine("Shape is hidden: " + shape.IsHidden);
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


