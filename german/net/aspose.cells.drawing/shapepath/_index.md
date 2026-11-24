---
title: "Klasse ShapePath"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.ShapePath Klasse. Stellt einen Erstellungs-Pfad dar, der aus einer Reihe von Bewegungen, Linien und Kurven besteht, die zusammen eine geometrische Form ergeben"
type: docs
url: /de/net/aspose.cells.drawing/shapepath/
---
## ShapePath class

Stellt einen Erstellungsweg dar, der aus einer Reihe von Bewegungen, Linien und Kurven besteht, die zusammen eine geometrische Form bilden.

```csharp
public class ShapePath
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [ShapePath](shapepath/)() | Initialisiert eine neue Instanz der `ShapePath` Klasse. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [HeightPixel](../../aspose.cells.drawing/shapepath/heightpixel/) { get; set; } | Liefert die Höhe dieses Pfads in Pixeln. |
| [PathSegementList](../../aspose.cells.drawing/shapepath/pathsegementlist/) { get; } | (**Veraltet.**) Liefert die [`ShapeSegmentPathCollection`](../shapesegmentpathcollection/) Liste |
| [PathSegments](../../aspose.cells.drawing/shapepath/pathsegments/) { get; } | Liefert die [`ShapeSegmentPathCollection`](../shapesegmentpathcollection/) Liste |
| [WidthPixel](../../aspose.cells.drawing/shapepath/widthpixel/) { get; set; } | Ermittelt die Breite dieses Pfads in Pixeln. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [ArcTo](../../aspose.cells.drawing/shapepath/arcto/)(float, float, float, float) | Fügt einen elliptischen Bogen zur aktuellen Figur hinzu. Der Startpunkt ist der Endpunkt der aktuellen Figur. |
| [Close](../../aspose.cells.drawing/shapepath/close/)() | Schließt die aktuelle Figur und startet eine neue Figur. Wenn die aktuelle Figur eine Sequenz verbundener Linien und Kurven enthält, schließt die Methode die Schleife, indem sie eine Linie vom Endpunkt zum Startpunkt verbindet. |
| [CubicBezierTo](../../aspose.cells.drawing/shapepath/cubicbezierto/)(float, float, float, float, float, float) | Fügt eine kubische Bézier-Kurve zur aktuellen Figur hinzu. Der Startpunkt ist der Endpunkt der aktuellen Figur. Einheit: Pixel. |
| [LineTo](../../aspose.cells.drawing/shapepath/lineto/)(float, float) | Fügt ein Liniensegment zur aktuellen Figur hinzu. Der Startpunkt ist der Endpunkt der aktuellen Figur. Einheit: Pixel. |
| [MoveTo](../../aspose.cells.drawing/shapepath/moveto/)(float, float) | Startet eine neue Figur vom angegebenen Punkt, ohne die aktuelle Figur zu schließen. Alle nachfolgenden Punkte, die dem Pfad hinzugefügt werden, werden zu dieser neuen Figur hinzugefügt. Einheit: Pixel. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassShapePathDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine benutzerdefinierte Form mit allen erforderlichen Parametern hinzu
            Shape customShape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 10, 10, 200, 100, 0, 0);
            
            // Greife auf die ShapePathCollection zu
            ShapePathCollection shapePaths = customShape.Paths;

            // Füge einen neuen Pfad hinzu und greife darauf zu
            int pathIndex = shapePaths.Add();
            ShapePath newPath = shapePaths[pathIndex];

            // Gib die Anzahl der Pfade aus
            Console.WriteLine("Number of paths in the ShapePathCollection: " + shapePaths.Count.ToString());

            // Speichere die Arbeitsmappe
            workbook.Save("ShapePathDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


