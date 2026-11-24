---
title: "Klasse ShapePathPoint"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.ShapePathPoint Klasse. Gibt Positionskoordinaten oder Winkelmarkierungen an. Positionskoordinaten stellen die Koordinaten eines Pfads in einem Koordinatenraum dar, z. B. X/Y. Winkelmarkierungen zeigen Winkeländerungen in einem Pfad an, z. B. die Start‑ und Schwenkwinkel eines Bogens."
type: docs
url: /de/net/aspose.cells.drawing/shapepathpoint/
---
## ShapePathPoint class

Geben Sie Positionskoordinaten oder Winkelmarkierungen an. Positionskoordinaten stellen die Koordinaten eines Pfads in einem Koordinatenraum dar (z. B. X/Y). Winkelmarkierungen zeigen Winkeländerungen in einem Pfad an (z. B. die Start- und Schwenkwinkel eines Bogens).

```csharp
public class ShapePathPoint
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Type](../../aspose.cells.drawing/shapepathpoint/type/) { get; } | Gibt den Werttyp des aktuellen Objekts an. |
| [X](../../aspose.cells.drawing/shapepathpoint/x/) { get; set; } | (**Obsolete.**) Liest und schreibt die x‑Koordinate für diese Positionskoordinate. Einheit EMUs. |
| [XAngle](../../aspose.cells.drawing/shapepathpoint/xangle/) { get; set; } | Wenn das Objekt ein Winkelmarker ist, lese oder schreibe den ersten Winkel in Grad. |
| [XPixel](../../aspose.cells.drawing/shapepathpoint/xpixel/) { get; set; } | Wenn das Objekt eine Positionskoordinate ist, lese oder schreibe die x‑Koordinate in Pixeln. |
| [Y](../../aspose.cells.drawing/shapepathpoint/y/) { get; set; } | (**Obsolete.**) Liest die y‑Koordinate für diese Positionskoordinate. Einheit EMUs. |
| [YAngle](../../aspose.cells.drawing/shapepathpoint/yangle/) { get; set; } | Wenn das Objekt ein Winkelmarker ist, lese oder schreibe den zweiten Winkel in Grad. |
| [YPixel](../../aspose.cells.drawing/shapepathpoint/ypixel/) { get; set; } | Wenn das Objekt eine Positionskoordinate ist, lese oder schreibe die y‑Koordinate in Pixeln. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassShapePathPointDemo
    {
        public static void Run()
        {
            // Erstellt ein neues Arbeitsbuch für die Demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Füge eine Form hinzu, die Pfadpunkte mit allen erforderlichen Parametern enthält
                Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 10, 10, 200, 200);
                
                // Lese die geometrischen Pfadpunkte
                CustomGeometry geometry = shape.Geometry as CustomGeometry;
                if (geometry != null && geometry.Paths.Count > 0)
                {
                    ShapePath path = geometry.Paths[0];
                    
                    // Greife auf einen vorhandenen Pfadpunkt zu (falls verfügbar)
                    if (path.PathSegementList.Count > 0)
                    {
                        // Lese den ersten Punkt (die tatsächliche Implementierung kann je nach Segmenttyp variieren)
                        ShapePathPoint point = path.PathSegementList[0].Points[0];
                        
                        // Zeige die Punktkoordinaten an
                        Console.WriteLine($"ShapePathPoint at X: {point.X}, Y: {point.Y}");
                    }
                }
                
                // Speichere die Arbeitsmappe
                workbook.Save("ShapePathPointDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ShapePathPoint: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


