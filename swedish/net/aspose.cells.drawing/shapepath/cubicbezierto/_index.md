---
title: "ShapePath.CubicBezierTo"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapePath metod. Lägger till en kubisk Bézier-kurva till den aktuella figuren. Startpunkten är slutpunkten för den aktuella figuren. Enhet Pixel"
type: docs
url: /sv/net/aspose.cells.drawing/shapepath/cubicbezierto/
---
## ShapePath.CubicBezierTo method

Lägger till en kubisk Bézier-kurva till den aktuella figuren. Startpunkten är slutpunkten för den aktuella figuren.Enhet: Pixel.

```csharp
public void CubicBezierTo(float ctrX1, float ctrY1, float ctrX2, float ctrY2, float endX, 
    float endY)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ctrX1 | Single | X-koordinaten för den första kontrollpunkten för kurvan (Enhet: Pixel). |
| ctrY1 | Single | Y-koordinaten för den första kontrollpunkten för kurvan (Enhet: Pixel). |
| ctrX2 | Single | X-koordinaten för den andra kontrollpunkten för kurvan (Enhet: Pixel). |
| ctrY2 | Single | Y-koordinaten för den andra kontrollpunkten för kurvan (Enhet: Pixel). |
| endX | Single | X-koordinaten för kurvans slutpunkt (Enhet: Pixel). |
| endY | Single | Y-koordinaten för kurvans slutpunkt (Enhet: Pixel). |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            //Skapa en ny formbana
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


            //lägg till fri form
            worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath1 });

            // Spara resultatet
            workbook.Save("ShapePathMethodCubicBezierToDemo.xlsx");
        }
    }
}
```

### Se även

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


