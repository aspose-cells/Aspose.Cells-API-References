---
title: "ShapePath.ArcTo"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapePath‑metod. Lägger till en elliptisk båge till den aktuella figuren. Startpunkten är slutpunkten för den aktuella figuren"
type: docs
url: /sv/net/aspose.cells.drawing/shapepath/arcto/
---
## ShapePath.ArcTo method

Lägger till en elliptisk båge till den aktuella figuren. Startpunkten är slutpunkten för den aktuella figuren.

```csharp
public void ArcTo(float wR, float hR, float stAng, float swAng)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| wR | Single | Halvbredden på det rektangulära området för ellipsen som ritar bågen (Enhet: Pixel). |
| hR | Single | Halvhöjden på det rektangulära området för ellipsen som ritar bågen (Enhet: Pixel). |
| stAng | Single | Startvinkeln för bågen, mätt i grader medurs från x‑axeln (Enhet: Grad). Denna vinkel anger vilken vinkel längs den antagna cirkelbanan som ska användas som startposition för att rita bågen. Denna startvinkel låses till den senast kända pennpositionen i shape path. Detta garanterar en kontinuerlig shape path. |
| swAng | Single | Svängvinkeln för en båge. Denna vinkel anger hur långt längs den antagna cirkelbanan bågen ska sträcka sig i vinkel. Förlängningen från startvinkeln sker alltid i medurs riktning runt den antagna cirkeln. (Enhet: Grad) |

### Exempel

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
            //Skapa en ny formbana
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

            Workbook workbook = new Workbook();

            //lägg till fri form
            workbook.Worksheets[0].Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath, shapePath1 });

            // Spara resultatet
            workbook.Save("ShapePathMethodArcToDemo.xlsx");
        }
    }
}
```

### Se även

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


