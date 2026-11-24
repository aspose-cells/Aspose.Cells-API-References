---
title: "CustomGeometry.Paths"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CustomGeometry-Eigenschaft. Ruft Pfadsammlungsinformationen ab, wenn die Form ein NotPrimitive autoshape ist."
type: docs
url: /de/net/aspose.cells.drawing/customgeometry/paths/
---
## CustomGeometry.Paths property

Ruft Pfadsammlungsinformationen ab, wenn die Form ein NotPrimitive-Autoshape ist

```csharp
public ShapePathCollection Paths { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class CustomGeometryPropertyPathsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie eine benutzerdefinierte Form mit nicht-primitiver Geometrie (feste Parameter) hinzu.
            var shape = worksheet.Shapes.AddAutoShape(AutoShapeType.NotPrimitive, 0, 0, 10, 10, 400, 400);
            
            // Greifen Sie über einen expliziten Cast auf die benutzerdefinierte Geometrie zu.
            CustomGeometry geometry = (CustomGeometry)shape.Geometry;
            
            // Pfadsammlung abrufen
            ShapePathCollection paths = geometry.Paths;
            Console.WriteLine($"Initial path count: {paths.Count}");

            // Erstellen Sie einen neuen Formpfad mithilfe von Zeichenbefehlen
            paths.Add(); // Creates a new path in the collection
            ShapePath newPath = paths[paths.Count - 1];
            newPath.MoveTo(0, 0);
            newPath.LineTo(10000, 0);
            newPath.LineTo(10000, 10000);
            newPath.LineTo(0, 10000);
            newPath.Close();

            // Kein explizites Hinzufügen erforderlich, da der Pfad in der Sammlung erstellt wurde
            Console.WriteLine($"New path count after modification: {paths.Count}");

            // Speichern, um dauerhafte Änderungen zu demonstrieren
            workbook.Save("CustomGeometryPathsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ShapePathCollection](../../shapepathcollection/)
* class [CustomGeometry](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


