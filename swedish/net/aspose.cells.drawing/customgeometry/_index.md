---
title: "Klass CustomGeometry"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.CustomGeometry-klass. Representerar en anpassad geometrisk form"
type: docs
url: /sv/net/aspose.cells.drawing/customgeometry/
---
## CustomGeometry class

Representerar en anpassad geometrisk form.

```csharp
public class CustomGeometry : Geometry
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Paths](../../aspose.cells.drawing/customgeometry/paths/) { get; } | Hämtar information om sökvägssamlingen när formen är en NotPrimitive-autoshape |
| [ShapeAdjustValues](../../aspose.cells.drawing/geometry/shapeadjustvalues/) { get; } | Hämtar en samling av formjusteringsvärden (ärvd från [`Geometry`](../geometry/).) |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassCustomGeometryDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en NotPrimitive-autoshape med korrekta parametrar
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.NotPrimitive, 0, 0, 0, 0, 200, 300);

            // Hämta CustomGeometry-instansen från formen
            CustomGeometry customGeometry = shape.Geometry as CustomGeometry;

            // Skapa en ny sökväg i geometrins sökvägssamling
            int pathIndex = customGeometry.Paths.Add();
            ShapePath path = customGeometry.Paths[pathIndex];

            // Lägg till sökvägssegment med direkta metodanrop
            path.MoveTo(0, 0);
            path.LineTo(1000, 0);
            path.LineTo(1000, 1000);
            path.LineTo(0, 1000);
            path.Close();

            // Spara arbetsboken
            workbook.Save("CustomGeometryDemo.xlsx");
        }
    }
}
```

### Se även

* class [Geometry](../geometry/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


