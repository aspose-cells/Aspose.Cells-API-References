---
title: "Enum ShapePathType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.ShapePathType enum. Representerar segmenttyp för sökväg"
type: docs
url: /sv/net/aspose.cells.drawing/shapepathtype/
---
## ShapePathType enumeration

Representerar typ av sökvägssegment.

```csharp
public enum ShapePathType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| LineTo | `1` | Rakt linjesegment |
| CubicBezierCurveTo | `3` | Kubisk Bezier-kurva |
| MoveTo | `0` | Starta en ny sökväg |
| Close | `128` | Om den startande POINT och den avslutande POINT inte är samma, ritas en enda rak linje för att ansluta den startande POINT och den avslutande POINT av sökvägen. |
| End | `4` | Slutet på den aktuella sökvägen |
| Escape | `5` | Avbryt |
| ArcTo | `6` | En båge |
| Unknown | `7` | Okänd |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassShapePathTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok för demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Skapa en form för att demonstrera sökvägstyper
                Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 10, 10, 10, 10, 200, 200);

                // Skapa en anpassad geometrisk sökväg
                Geometry geometry = shape.Geometry;
                ShapePath path = new ShapePath();

                // Demonstrera olika ShapePathType‑värden
                Console.WriteLine("Available ShapePathType values:");
                Console.WriteLine($"LineTo: {ShapePathType.LineTo}");
                Console.WriteLine($"CubicBezierCurveTo: {ShapePathType.CubicBezierCurveTo}");
                Console.WriteLine($"MoveTo: {ShapePathType.MoveTo}");
                Console.WriteLine($"Close: {ShapePathType.Close}");
                Console.WriteLine($"End: {ShapePathType.End}");

                // Applicera några sökvägsoperationer
                path.MoveTo(10, 10);
                path.LineTo(100, 100);
                path.Close();

                // Spara arbetsboken
                workbook.Save("ShapePathTypeDemo.xlsx");
                Console.WriteLine("Demo completed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ShapePathType: {ex.Message}");
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


