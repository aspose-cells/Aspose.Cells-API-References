---
title: "Shape.Line"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Hämtar linjestil"
type: docs
url: /sv/net/aspose.cells.drawing/shape/line/
---
## Shape.Line property

Hämtar linjestil

```csharp
public LineFormat Line { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLineDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en linjeform (returnerar LineShape direkt)
            LineShape lineShape = worksheet.Shapes.AddLine(1, 0, 1, 0, 5, 100);

            // Kom åt och ändra linjeegenskaper
            LineFormat lineFormat = lineShape.Line;
            lineFormat.CompoundType = MsoLineStyle.ThickThin;
            lineFormat.DashStyle = MsoLineDashStyle.DashDot;
            lineFormat.Weight = 3.0;
            lineFormat.BeginArrowheadStyle = MsoArrowheadStyle.Arrow;
            lineFormat.EndArrowheadStyle = MsoArrowheadStyle.ArrowOpen;

            // Spara arbetsboken
            workbook.Save("LineShapeDemo.xlsx");
        }
    }
}
```

### Se även

* class [LineFormat](../../lineformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


