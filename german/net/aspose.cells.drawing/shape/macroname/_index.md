---
title: "Shape.MacroName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Liest und setzt den Namen des Makros"
type: docs
url: /de/net/aspose.cells.drawing/shape/macroname/
---
## Shape.MacroName property

Liest und setzt den Namen des Makros.

```csharp
public string MacroName { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt eine Form hinzu
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Setze den Makronamen für die Form
            shape.MacroName = "DoWork()";

            // Ausgabebestätigung
            Console.WriteLine("Shape macro name set to: " + shape.MacroName);
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


