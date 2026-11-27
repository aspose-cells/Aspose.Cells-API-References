---
title: "Klass Geometry"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.Geometry-klass. Representerar en geometrisk form"
type: docs
url: /sv/net/aspose.cells.drawing/geometry/
---
## Geometry class

Representerar en geometrisk form.

```csharp
public abstract class Geometry
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [ShapeAdjustValues](../../aspose.cells.drawing/geometry/shapeadjustvalues/) { get; } | Hämtar en samling av justeringsvärden för formen |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    
    public class DrawingClassGeometryDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform i arbetsbladet
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 200);

            // Åtkomst till geometrin för formen
            Geometry geometry = rectangle.Geometry;

            // Lägg till justeringsguider för formen direkt i samlingen
            geometry.ShapeAdjustValues.Add("Roundness", 0.3);
            geometry.ShapeAdjustValues.Add("Angle", 45.0);

            // Spara den modifierade arbetsboken
            workbook.Save("GeometryDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


