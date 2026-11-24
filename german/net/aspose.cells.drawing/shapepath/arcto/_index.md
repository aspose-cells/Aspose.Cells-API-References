---
title: "ShapePath.ArcTo"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapePath-Methode. Fügt einen elliptischen Bogen zur aktuellen Figur hinzu. Der Startpunkt ist der Endpunkt der aktuellen Figur"
type: docs
url: /de/net/aspose.cells.drawing/shapepath/arcto/
---
## ShapePath.ArcTo method

Fügt einen elliptischen Bogen zur aktuellen Figur hinzu. Der Startpunkt ist der Endpunkt der aktuellen Figur.

```csharp
public void ArcTo(float wR, float hR, float stAng, float swAng)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| wR | Einzeln | Die halbe Breite des rechteckigen Bereichs der Ellipse, die den Bogen zeichnet (Einheit: Pixel). |
| hR | Einzeln | Die halbe Höhe des rechteckigen Bereichs der Ellipse, die den Bogen zeichnet (Einheit: Pixel). |
| stAng | Einzeln | Der Startwinkel des Bogens, gemessen in Grad im Uhrzeigersinn von der x-Achse (Einheit: Grad). Dieser Winkel gibt an, welcher Winkel entlang des angenommenen Kreiswegs als Startposition für das Zeichnen des Bogens verwendet wird. Dieser Startwinkel wird an die zuletzt bekannte Stiftposition im ShapePath gesperrt. Dadurch wird ein kontinuierlicher ShapePath garantiert. |
| swAng | Einzeln | Der Schwenkwinkel für einen Bogen. Dieser Winkel gibt an, wie weit entlang des angenommenen Kreiswegs der Bogen ausgedehnt wird. Die Erweiterung vom Startwinkel erfolgt immer im Uhrzeigersinn um den angenommenen Kreis. (Einheit: Grad) |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodArcToWithSingleSingleSingleSingleDemo
    {
        public static void Run()
        {
            //Erstellen Sie einen neuen Formpfad
            ShapePath shapePath = new ShapePath();
            shapePath.MoveTo(60, 45);
            shapePath.ArcTo(25, 25, 0, 270);
            shapePath.Close();

            shapePath.MoveTo(60, 20);
            shapePath.LineTo(110, 70);
            shapePath.LineTo(125, 155.5f);
            shapePath.ArcTo(35.5f, 35.5f, 0, 270);
            shapePath.Close();

            shapePath.MoveTo(150, 45);
            shapePath.ArcTo(25, 25, 0, 270);

            //Erstellen Sie einen neuen Formpfad
            ShapePath shapePath1 = new ShapePath();
            shapePath1.MoveTo(0, 0);
            shapePath1.CubicBezierTo(48.24997f, 0.6844f,
                        96.5f, -7.148871f,
                        130, 11.517795f);
            shapePath1.CubicBezierTo(163.5f, 30.18446f,
                        182.24997f, 75.351f,
                        201, 120.517795f);
            shapePath1.MoveTo(150, 70);
            shapePath1.ArcTo(25, 25, 0, 270);

            Workbook workbook = new Workbook();

            //Freiform hinzufügen
            workbook.Worksheets[0].Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath, shapePath1 });

            // Ergebnis speichern
            workbook.Save("ShapePathMethodArcToDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


