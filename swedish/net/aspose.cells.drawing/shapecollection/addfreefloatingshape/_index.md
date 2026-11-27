---
title: "ShapeCollection.AddFreeFloatingShape"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeCollection-metod. Lägger till en fritt flytande shape i kalkylbladet. Gäller endast för linje-/bildshape"
type: docs
url: /sv/net/aspose.cells.drawing/shapecollection/addfreefloatingshape/
---
## ShapeCollection.AddFreeFloatingShape method

Lägger till en fritt flytande shape i kalkylbladet. Gäller endast för linje-/bildshape.

```csharp
public Shape AddFreeFloatingShape(MsoDrawingType type, int top, int left, int height, int width, 
    byte[] imageData, bool isOriginalSize)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | MsoDrawingType | Shape-typen. |
| top | Int32 | Representerar den vertikala förskjutningen för shape från kalkylbladets översta rad, i enheten pixel. |
| vänster | Int32 | Representerar den horisontella förskjutningen för shape från kalkylbladets vänstra kolumn, i enheten pixel. |
| höjd | Int32 | Representerar höjden på LineShape, i enheten pixel. |
| bredd | Int32 | Representerar bredden på LineShape, i enheten pixel. |
| imageData | Byte[] | Bilddata, gäller endast för bilden. |
| isOriginalSize | Boolean | Anger om shape använder originalstorlek om shape är en bild. |

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddFreeFloatingShapeWithMsoDrawingTypeInt32Int32Int32IDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            // Lägg till en linjeform
            Shape floatingShape_Line = shapes.AddFreeFloatingShape(
                MsoDrawingType.Line, 
                100, 100, 100, 50, 
                null, 
                false);

            // Lägg till en picture-shape (med exempelbilddata)
            byte[] imageData = null;
            try
            {
                using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
                {
                    imageData = new byte[fs.Length];
                    fs.Read(imageData, 0, (int)fs.Length);
                }
            }
            catch
            {
                // Skapa dummy-bilddata om filen inte hittas
                imageData = new byte[100];
            }

            Shape floatingShape_Picture = shapes.AddFreeFloatingShape(
                MsoDrawingType.Picture, 
                200, 100, 100, 50, 
                imageData, 
                false);

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Shape](../../shape/)
* enum [MsoDrawingType](../../msodrawingtype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


