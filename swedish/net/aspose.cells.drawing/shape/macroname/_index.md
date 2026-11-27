---
title: "Shape.MacroName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape property. Hämtar och anger namnet på makrot"
type: docs
url: /sv/net/aspose.cells.drawing/shape/macroname/
---
## Shape.MacroName property

Hämtar och anger namnet på makrot.

```csharp
public string MacroName { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyMacroNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form i kalkylbladet
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Ange makronamnet för formen
            shape.MacroName = "DoWork()";

            // Skriv ut bekräftelse
            Console.WriteLine("Shape macro name set to: " + shape.MacroName);
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


