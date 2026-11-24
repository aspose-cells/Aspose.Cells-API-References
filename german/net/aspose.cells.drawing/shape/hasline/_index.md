---
title: "Shape.HasLine"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt an, ob die Linienbegrenzung der Form sichtbar ist, und legt sie fest"
type: docs
url: /de/net/aspose.cells.drawing/shape/hasline/
---
## Shape.HasLine property

Ermittelt und setzt, ob die Linienbegrenzung der Form sichtbar ist.

```csharp
public bool HasLine { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispielhafte Form mit allen erforderlichen Parametern hinzufügen
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            // Demonstriere die HasLine-Eigenschaft
            Console.WriteLine("Shape initially has line: " + shape.HasLine);
            
            // Entferne die Linie
            shape.HasLine = false;
            Console.WriteLine("After setting HasLine to false: " + shape.HasLine);
            
            // Füge die Linie wieder hinzu
            shape.HasLine = true;
            Console.WriteLine("After setting HasLine to true: " + shape.HasLine);
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


