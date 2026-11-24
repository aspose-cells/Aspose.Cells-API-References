---
title: "Klasse CustomGeometry"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.CustomGeometry Klasse. Stellt eine benutzerdefinierte geometrische Form dar"
type: docs
url: /de/net/aspose.cells.drawing/customgeometry/
---
## CustomGeometry class

Stellt eine benutzerdefinierte geometrische Form dar.

```csharp
public class CustomGeometry : Geometry
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Paths](../../aspose.cells.drawing/customgeometry/paths/) { get; } | Ruft Pfadsammlungsinformationen ab, wenn die Form ein NotPrimitive-Autoshape ist |
| [ShapeAdjustValues](../../aspose.cells.drawing/geometry/shapeadjustvalues/) { get; } | Ruft eine Sammlung von Form‑Anpassungswerten ab (geerbt von [`Geometry`](../geometry/).) |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie ein NotPrimitive-Autoshape mit korrekten Parametern hinzu
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.NotPrimitive, 0, 0, 0, 0, 200, 300);

            // Holen Sie die CustomGeometry-Instanz aus der Form
            CustomGeometry customGeometry = shape.Geometry as CustomGeometry;

            // Erstellen Sie einen neuen Pfad in der Pfadsammlung der Geometrie
            int pathIndex = customGeometry.Paths.Add();
            ShapePath path = customGeometry.Paths[pathIndex];

            // Fügen Sie Pfadsegmente mit direkten Methodenaufrufen hinzu
            path.MoveTo(0, 0);
            path.LineTo(1000, 0);
            path.LineTo(1000, 1000);
            path.LineTo(0, 1000);
            path.Close();

            // Speichere die Arbeitsmappe
            workbook.Save("CustomGeometryDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Geometry](../geometry/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


