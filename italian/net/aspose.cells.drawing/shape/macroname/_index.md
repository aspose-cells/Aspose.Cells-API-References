---
title: "Shape.MacroName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Ottiene e imposta il nome della macro"
type: docs
url: /it/net/aspose.cells.drawing/shape/macroname/
---
## Shape.MacroName property

Ottiene e imposta il nome della macro.

```csharp
public string MacroName { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma al foglio di lavoro
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Imposta il nome della macro per la forma
            shape.MacroName = "DoWork()";

            // Conferma dell'output
            Console.WriteLine("Shape macro name set to: " + shape.MacroName);
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


