---
title: "ScrollBar.Min"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ScrollBar-egenskap. Hämtar eller anger det minsta värdet för ett rullningsfält eller en spinnerintervall"
type: docs
url: /sv/net/aspose.cells.drawing/scrollbar/min/
---
## ScrollBar.Min property

Hämtar eller anger det minsta värdet för ett rullningslist‑ eller spinnerintervall.

```csharp
public int Min { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ScrollBarPropertyMinDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till ett rullningsfält i kalkylbladet
            Aspose.Cells.Drawing.ScrollBar scrollBar = (Aspose.Cells.Drawing.ScrollBar)worksheet.Shapes.AddScrollBar(1, 0, 1, 1, 100, 20);

            // Ställ in rullningsfältsegenskaper
            scrollBar.Min = 10;
            scrollBar.Max = 100;
            scrollBar.CurrentValue = 50;  // Changed from Value to CurrentValue
            scrollBar.IncrementalChange = 5;
            scrollBar.PageChange = 20;

            // Visa värdet för Min-egenskapen
            Console.WriteLine("ScrollBar Min Value: " + scrollBar.Min);

            // Spara arbetsboken
            workbook.Save("ScrollBarMinDemo.xlsx");
        }
    }
}
```

### Se även

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


