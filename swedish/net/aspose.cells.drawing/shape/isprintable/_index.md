---
title: "Shape.IsPrintable"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Anger om objektet är utskrivbart. Om False kommer denna form inte att skrivas ut vid utskrift"
type: docs
url: /sv/net/aspose.cells.drawing/shape/isprintable/
---
## Shape.IsPrintable property

Anger om objektet är utskrivbart. Om falskt kommer denna form inte att skrivas ut vid utskrift.

```csharp
public bool IsPrintable { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsPrintableDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form i kalkylbladet
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Demonstrera egenskapen IsPrintable
            Console.WriteLine("Shape is printable initially: " + shape.IsPrintable);

            // Växla egenskapen IsPrintable
            shape.IsPrintable = !shape.IsPrintable;
            Console.WriteLine("Shape is printable after toggle: " + shape.IsPrintable);

            // Ställ in IsPrintable till false uttryckligen
            shape.IsPrintable = false;
            Console.WriteLine("Shape is printable after setting to false: " + shape.IsPrintable);
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


