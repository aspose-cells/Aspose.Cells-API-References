---
title: "Klass ShapeSegmentPath"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.ShapeSegmentPath klass. Representerar en segmentbana i en bana för frihandsformen"
type: docs
url: /sv/net/aspose.cells.drawing/shapesegmentpath/
---
## ShapeSegmentPath class

Representerar en segmentbana i en bana för frihandsformen.

```csharp
public class ShapeSegmentPath
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Points](../../aspose.cells.drawing/shapesegmentpath/points/) { get; } | Hämtar punkterna i vägsegmentet |
| [Type](../../aspose.cells.drawing/shapesegmentpath/type/) { get; } | Hämtar typen av vägsegmentet |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassShapeSegmentPathDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en frihandsform i arbetsbladet
            Shape shape = worksheet.Shapes.AddFreeform(0, 0, 0, 0, 200, 200, new ShapePath[] { new ShapePath() });

            // Hämta geometribanan för formen
            CustomGeometry geometry = shape.Geometry as CustomGeometry;
            ShapePath shapePath = geometry.Paths[0];

            // Få åtkomst till den första segmentbanan (om den finns)
            if (shapePath.PathSegementList.Count > 0)
            {
                ShapeSegmentPath segmentPath = shapePath.PathSegementList[0];

                // Visa egenskaperna för ShapeSegmentPath
                Console.WriteLine("Segment Path Type: " + segmentPath.Type);
                Console.WriteLine("Number of Points: " + segmentPath.Points.Count);

                // Iterera genom punkterna i segmentbanan
                foreach (ShapePathPoint point in segmentPath.Points)
                {
                    Console.WriteLine($"Point coordinates: X={point.X}, Y={point.Y}");
                }
            }

            // Spara arbetsboken
            workbook.Save("ShapeSegmentPathDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


