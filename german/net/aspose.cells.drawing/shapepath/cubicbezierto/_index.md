---
title: "ShapePath.CubicBezierTo"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapePath‑Methode. Fügt der aktuellen Figur eine kubische Bézier‑Kurve hinzu. Der Startpunkt ist der Endpunkt der aktuellen Figur. Einheit Pixel"
type: docs
url: /de/net/aspose.cells.drawing/shapepath/cubicbezierto/
---
## ShapePath.CubicBezierTo method

Fügt eine kubische Bézier-Kurve zur aktuellen Figur hinzu. Der Startpunkt ist der Endpunkt der aktuellen Figur. Einheit: Pixel.

```csharp
public void CubicBezierTo(float ctrX1, float ctrY1, float ctrX2, float ctrY2, float endX, 
    float endY)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| ctrX1 | Einzeln | Die x‑Koordinate des ersten Kontrollpunkts der Kurve (Einheit: Pixel). |
| ctrY1 | Einzeln | Die y‑Koordinate des ersten Kontrollpunkts der Kurve (Einheit: Pixel). |
| ctrX2 | Einzeln | Die x‑Koordinate des zweiten Kontrollpunkts der Kurve (Einheit: Pixel). |
| ctrY2 | Einzeln | Die y‑Koordinate des zweiten Kontrollpunkts der Kurve (Einheit: Pixel). |
| endX | Einzeln | Die x‑Koordinate des Endpunkts der Kurve (Einheit: Pixel). |
| endY | Einzeln | Die y‑Koordinate des Endpunkts der Kurve (Einheit: Pixel). |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodCubicBezierToWithSingleSingleSingleSingleSingleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

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


            //Freiform hinzufügen
            worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath1 });

            // Ergebnis speichern
            workbook.Save("ShapePathMethodCubicBezierToDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


