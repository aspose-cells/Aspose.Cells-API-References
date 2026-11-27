---
title: "ShapeCollection.AddAutoShape"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeCollection-metod. Lägger till en AutoShape i kalkylbladet"
type: docs
url: /sv/net/aspose.cells.drawing/shapecollection/addautoshape/
---
## ShapeCollection.AddAutoShape method

Lägger till en AutoShape i kalkylbladet.

```csharp
public Shape AddAutoShape(AutoShapeType type, int topRow, int top, int leftColumn, int left, 
    int height, int width)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | AutoShapeType | Auto shape-typ. |
| topRow | Int32 | Övre vänstra radindex. |
| top | Int32 | Representerar den vertikala förskjutningen av Shape från dess vänstra rad, i enheten pixel. |
| leftColumn | Int32 | Övre vänstra kolumnindex. |
| vänster | Int32 | Representerar den horisontella förskjutningen av Shape från dess vänstra kolumn, i enheten pixel. |
| höjd | Int32 | Representerar höjden på Shape, i enheten pixel. |
| bredd | Int32 | Representerar bredden på Shape, i enheten pixel. |

### Returvärde

Ett Shape-objekt.

### Anmärkningar

Typen kunde inte vara Chart/Comment/Picture/OleObject/Polygon/DialogBox

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddAutoShapeWithAutoShapeTypeInt32Int32Int32InDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            ShapeCollection shapes = worksheet.Shapes;
            Shape autoShape = shapes.AddAutoShape(AutoShapeType.Cube, 1, 0, 1, 0, 100, 50);
            
            workbook.Save("AutoShapeDemo.xlsx");
        }
    }
}
```

### Se även

* class [Shape](../../shape/)
* enum [AutoShapeType](../../autoshapetype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


