---
title: "Shape.WidthInShape"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Representerar bredden på formen i enheten 1/4000 av föräldraformen"
type: docs
url: /sv/net/aspose.cells.drawing/shape/widthinshape/
---
## Shape.WidthInShape property

Representerar formens bredd, i enhet av 1/4000 av föräldraformen.

```csharp
public int WidthInShape { get; set; }
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
    public class ShapePropertyWidthInShapeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa två rektangelformer
            Shape rect1 = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 100);
            Shape rect2 = worksheet.Shapes.AddRectangle(0, 100, 0, 0, 100, 100);
            
            // Gruppera formerna med hjälp av shape-objekt
            GroupShape group = worksheet.Shapes.Group(new Shape[] { rect1, rect2 });
            
            // Demonstrera användning av WidthInShape
            if (rect1.IsInGroup && rect1.WidthInShape == 2000)
            {
                rect1.WidthInShape = 4000;
            }
            
            // Spara modifierad arbetsbok
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


