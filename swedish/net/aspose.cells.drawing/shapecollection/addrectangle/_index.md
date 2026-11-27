---
title: "ShapeCollection.AddRectangle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeCollection-metod. Lägger till en RectangleShape i kalkylbladet"
type: docs
url: /sv/net/aspose.cells.drawing/shapecollection/addrectangle/
---
## ShapeCollection.AddRectangle method

Lägger till en rektangelform i kalkylbladet.

```csharp
public RectangleShape AddRectangle(int topRow, int top, int leftColumn, int left, int height, 
    int width)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | Int32 | Övre vänstra radindex. |
| top | Int32 | Representerar det vertikala offsetet för RectangleShape från dess vänstra rad, i enhet pixel. |
| leftColumn | Int32 | Övre vänstra kolumnindex. |
| vänster | Int32 | Representerar den horisontella förskjutningen av RectangleShape från dess vänstra kolumn, i enhet pixel. |
| höjd | Int32 | Representerar höjden på RectangleShape, i enhet pixel. |
| bredd | Int32 | Representerar bredden på RectangleShape, i enhet pixel. |

### Returvärde

Ett RectangleShape-objekt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddRectangleWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangel med de angivna parametrarna
            RectangleShape rectangleShape = worksheet.Shapes.AddRectangle(2, 0, 2, 0, 130, 130);

            // Spara arbetsboken
            workbook.Save("RectangleShapeDemo.xlsx");
        }
    }
}
```

### Se även

* class [RectangleShape](../../rectangleshape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


