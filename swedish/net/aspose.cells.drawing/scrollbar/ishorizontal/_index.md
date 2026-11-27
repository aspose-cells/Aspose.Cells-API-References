---
title: "ScrollBar.IsHorizontal"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ScrollBar-egenskap. Anger om detta är ett horisontellt rullningsfält"
type: docs
url: /sv/net/aspose.cells.drawing/scrollbar/ishorizontal/
---
## ScrollBar.IsHorizontal property

Anger om detta är en horisontell rullningslist.

```csharp
public bool IsHorizontal { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ScrollBarPropertyIsHorizontalDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en horisontell rullningslist
            Shape scrollBarShape = worksheet.Shapes.AddScrollBar(1, 0, 1, 0, 100, 20);
            ScrollBar scrollBar = (ScrollBar)scrollBarShape;
            scrollBar.IsHorizontal = true;

            // Lägg till ett vertikalt rullningsfält för jämförelse
            Shape verticalScrollBarShape = worksheet.Shapes.AddScrollBar(1, 0, 1, 30, 20, 100);
            ScrollBar verticalScrollBar = (ScrollBar)verticalScrollBarShape;
            verticalScrollBar.IsHorizontal = false;

            // Demonstrera IsHorizontal-egenskapen
            Console.WriteLine("Horizontal Scroll Bar IsHorizontal: " + scrollBar.IsHorizontal);
            Console.WriteLine("Vertical Scroll Bar IsHorizontal: " + verticalScrollBar.IsHorizontal);

            // Spara arbetsboken
            workbook.Save("ScrollBarDemo.xlsx");
        }
    }
}
```

### Se även

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


