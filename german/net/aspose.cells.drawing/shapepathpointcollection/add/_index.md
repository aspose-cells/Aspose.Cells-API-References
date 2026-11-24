---
title: "ShapePathPointCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapePathPointCollection-Methode. Fügt einen Pfadpunkt in EMU-Einheiten hinzu"
type: docs
url: /de/net/aspose.cells.drawing/shapepathpointcollection/add/
---
## ShapePathPointCollection.Add method

Fügt einen Pfadpunkt in EMU-Einheiten hinzu.

```csharp
[Obsolete("Use the MoveTo,LineTo,CubicBezierTo and ArcTo methods in ShapePath instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(int x, int y)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| x | Int32 | Die x-Koordinate. |
| y | Int32 | Die y-Koordinate. |

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Methoden MoveTo,LineTo,CubicBezierTo und ArcTo in ShapePath. Diese Methode wird 12 Monate später ab August 2025 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointCollectionMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstellen Sie eine ShapePathPoint-Punktesammlung
            ShapePathPointCollection pathPoints = new ShapePathPointCollection();

            try
            {
                // Rufe die Add-Methode mit den Parametern (Int32, Int32) auf
                pathPoints.Add(50, 10);
                pathPoints.Add(50, 50);
                pathPoints.Add(10, 50);

                // Erstelle einen Formpfad und füge die Punkte hinzu
                ShapePath path = new ShapePath();

                // Zum Ausgangspunkt bewegen
                path.MoveTo(10, 10);

                foreach (ShapePathPoint point in pathPoints)
                {
                    path.LineTo(point.X, point.Y);
                }
                path.Close();

                // Fügen Sie eine Freihandform mit dem konfigurierten Pfad hinzu
                Shape shape = worksheet.Shapes.AddFreeform(
                    topRow: 2,
                    top: 0,
                    leftColumn: 2,
                    left: 0,
                    height: 200,
                    width: 200,
                    paths: new ShapePath[] { path }
                );

                // Ergebnis speichern
                workbook.Save("ShapePathPointCollectionMethodAddWithInt32Int32Demo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [ShapePathPointCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


