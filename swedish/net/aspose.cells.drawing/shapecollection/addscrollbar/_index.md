---
title: "ShapeCollection.AddScrollBar"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeCollection‑metod. Lägger till en ScrollBar i kalkylbladet"
type: docs
url: /sv/net/aspose.cells.drawing/shapecollection/addscrollbar/
---
## ShapeCollection.AddScrollBar method

Lägger till en rullningslist i kalkylbladet.

```csharp
public ScrollBar AddScrollBar(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | Int32 | Övre vänstra radindex. |
| top | Int32 | Representerar det vertikala avståndet för ScrollBar från dess vänstra rad, i enhet pixel. |
| leftColumn | Int32 | Övre vänstra kolumnindex. |
| vänster | Int32 | Representerar det horisontella avståndet för ScrollBar från dess vänstra kolumn, i enhet pixel. |
| höjd | Int32 | Representerar höjden på ScrollBar, i enhet pixel. |
| bredd | Int32 | Representerar bredden på ScrollBar, i enhet pixel. |

### Returvärde

Ett ScrollBar‑objekt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddScrollBarWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            ScrollBar scrollBar = shapes.AddScrollBar(1, 0, 100, 20, 0, 100);
            scrollBar.CurrentValue = 50;
            scrollBar.Width = 200;
            scrollBar.Height = 30;

            workbook.Save("ScrollBarDemo.xlsx");
        }
    }
}
```

### Se även

* class [ScrollBar](../../scrollbar/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


