---
title: "CustomGeometry.Paths"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CustomGeometry property. Hämtar information om sökvägssamlingen när formen är en NotPrimitive autoshape"
type: docs
url: /sv/net/aspose.cells.drawing/customgeometry/paths/
---
## CustomGeometry.Paths property

Hämtar information om sökvägssamlingen när formen är en NotPrimitive-autoshape

```csharp
public ShapePathCollection Paths { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en anpassad form med icke-primitive geometri (fasta parametrar)
            var shape = worksheet.Shapes.AddAutoShape(AutoShapeType.NotPrimitive, 0, 0, 10, 10, 400, 400);
            
            // Åtkomst till anpassad geometri via explicit castning
            CustomGeometry geometry = (CustomGeometry)shape.Geometry;
            
            // Hämta sökvägssamlingen
            ShapePathCollection paths = geometry.Paths;
            Console.WriteLine($"Initial path count: {paths.Count}");

            // Skapa en ny shape path med ritkommandon
            paths.Add(); // Creates a new path in the collection
            ShapePath newPath = paths[paths.Count - 1];
            newPath.MoveTo(0, 0);
            newPath.LineTo(10000, 0);
            newPath.LineTo(10000, 10000);
            newPath.LineTo(0, 10000);
            newPath.Close();

            // Ingen explicit Add behövs eftersom sökvägen skapades i samlingen
            Console.WriteLine($"New path count after modification: {paths.Count}");

            // Spara för att demonstrera bestående ändringar
            workbook.Save("CustomGeometryPathsDemo.xlsx");
        }
    }
}
```

### Se även

* class [ShapePathCollection](../../shapepathcollection/)
* class [CustomGeometry](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


