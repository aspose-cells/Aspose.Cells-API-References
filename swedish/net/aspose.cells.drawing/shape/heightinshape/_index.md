---
title: "Shape.HeightInShape"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Representerar det vertikala avståndet för formen från den övre kanten av föräldraformen i enhet av 1/4000 av föräldraformens höjd."
type: docs
url: /sv/net/aspose.cells.drawing/shape/heightinshape/
---
## Shape.HeightInShape property

Representerar den vertikala förskjutningen av formen från den översta kanten av föräldraformen, i enheten 1/4000 av föräldraformens höjd.

```csharp
public int HeightInShape { get; set; }
```

### Anmärkningar

Gäller endast när denna form är i gruppen eller diagrammet.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHeightInShapeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till former först med alla nödvändiga parametrar
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 10, 10);
            Shape oval = worksheet.Shapes.AddOval(0, 0, 100, 100, 10, 120);

            // Gruppera formerna
            Shape[] shapes = { rectangle, oval };
            GroupShape groupShape = worksheet.Shapes.Group(shapes);

            // Ställ in rektangelns höjd relativt till den överordnade gruppformen (1/4000 av förälderns höjd)
            rectangle.HeightInShape = 2000; // Half the height of the parent
            oval.HeightInShape = 4000; // Full height of the parent

            // Spara arbetsboken
            workbook.Save("ShapeHeightInShapeDemo.xlsx");
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


