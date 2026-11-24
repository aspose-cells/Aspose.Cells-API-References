---
title: "Klasse Geometry"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.Geometry Klasse. Stellt eine geometrische Form dar"
type: docs
url: /de/net/aspose.cells.drawing/geometry/
---
## Geometry class

Stellt eine geometrische Form dar.

```csharp
public abstract class Geometry
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [ShapeAdjustValues](../../aspose.cells.drawing/geometry/shapeadjustvalues/) { get; } | Ruft eine Sammlung von Formanpassungswerten ab |

### Beispiele

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

            // Füge ein Rechteck-Shape zum Arbeitsblatt hinzu
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 200);

            // Greifen Sie auf die Geometrie der Form zu
            Geometry geometry = rectangle.Geometry;

            // Fügen Sie Formanpassungsführungen direkt zur Sammlung hinzu
            geometry.ShapeAdjustValues.Add("Roundness", 0.3);
            geometry.ShapeAdjustValues.Add("Angle", 45.0);

            // Speichere die geänderte Arbeitsmappe
            workbook.Save("GeometryDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


