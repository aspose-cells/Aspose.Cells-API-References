---
title: "Shape.WidthInShape"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Stellt die Breite der Form in der Einheit 1/4000 der übergeordneten Form dar"
type: docs
url: /de/net/aspose.cells.drawing/shape/widthinshape/
---
## Shape.WidthInShape property

Stellt die Breite der Form dar, in Einheiten von 1/4000 der übergeordneten Form.

```csharp
public int WidthInShape { get; set; }
```

### Hinweise

Gilt nur, wenn diese Form in einer Gruppe oder einem Diagramm ist.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyWidthInShapeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstelle zwei Rechteckformen
            Shape rect1 = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 100);
            Shape rect2 = worksheet.Shapes.AddRectangle(0, 100, 0, 0, 100, 100);
            
            // Gruppiere die Formen mithilfe von Shape-Objekten
            GroupShape group = worksheet.Shapes.Group(new Shape[] { rect1, rect2 });
            
            // Demonstriere die Verwendung von WidthInShape
            if (rect1.IsInGroup && rect1.WidthInShape == 2000)
            {
                rect1.WidthInShape = 4000;
            }
            
            // Modifizierte Arbeitsmappe speichern
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


