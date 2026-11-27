---
title: "Enum ShapeAnchorType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.ShapeAnchorType enum. Representerar ankartypen"
type: docs
url: /sv/net/aspose.cells.drawing/shapeanchortype/
---
## ShapeAnchorType enumeration

Representerar ankartypen.

```csharp
public enum ShapeAnchorType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| TwoCellAnchor | `0` | Representerar en platshållare för två cellers ankare |
| OneCellAnchor | `1` | Representerar en platshållare för ett cellankare |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassShapeAnchorTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en gruppboxform
            Shape box = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 300, 250);
            box.Text = "Sample Group Box";
            
            // Demonstrera användning av ShapeAnchorType
            box.AnchorType = ShapeAnchorType.TwoCellAnchor;
            box.UpperLeftRow = 2;
            box.UpperLeftColumn = 1;
            box.LowerRightRow = 8;
            box.LowerRightColumn = 4;

            // Spara arbetsboken
            workbook.Save("ShapeAnchorTypeDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


