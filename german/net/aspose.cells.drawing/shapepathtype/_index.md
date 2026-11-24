---
title: "Aufzählung ShapePathType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.ShapePathType enum. Stellt den Pfadsegmenttyp dar"
type: docs
url: /de/net/aspose.cells.drawing/shapepathtype/
---
## ShapePathType enumeration

Stellt den Pfadsegmenttyp dar.

```csharp
public enum ShapePathType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| LineTo | `1` | Gerader Linienabschnitt |
| CubicBezierCurveTo | `3` | Kubische Bézier-Kurve |
| MoveTo | `0` | Beginnen Sie einen neuen Pfad |
| Close | `128` | Wenn der startende POINT und der end POINT nicht identisch sind, wird eine einzelne gerade Linie gezeichnet, um den startenden POINT und den end POINT des Pfades zu verbinden. |
| End | `4` | Das Ende des aktuellen Pfades |
| Escape | `5` | Entkommen |
| ArcTo | `6` | Ein Bogen |
| Unknown | `7` | Unbekannt |

### Beispiele

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
            // Erstellt ein neues Arbeitsbuch für die Demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Erstelle eine Form, um Pfadtypen zu demonstrieren
                Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 10, 10, 10, 10, 200, 200);

                // Erstelle einen benutzerdefinierten Geometriepfad
                Geometry geometry = shape.Geometry;
                ShapePath path = new ShapePath();

                // Demonstriere verschiedene ShapePathType-Werte
                Console.WriteLine("Available ShapePathType values:");
                Console.WriteLine($"LineTo: {ShapePathType.LineTo}");
                Console.WriteLine($"CubicBezierCurveTo: {ShapePathType.CubicBezierCurveTo}");
                Console.WriteLine($"MoveTo: {ShapePathType.MoveTo}");
                Console.WriteLine($"Close: {ShapePathType.Close}");
                Console.WriteLine($"End: {ShapePathType.End}");

                // Wende einige Pfadoperationen an
                path.MoveTo(10, 10);
                path.LineTo(100, 100);
                path.Close();

                // Speichere die Arbeitsmappe
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

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


