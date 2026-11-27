---
title: "ScrollBar.CurrentValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ScrollBar-egenskap. Hämtar eller anger det aktuella värdet"
type: docs
url: /sv/net/aspose.cells.drawing/scrollbar/currentvalue/
---
## ScrollBar.CurrentValue property

Hämtar eller anger det aktuella värdet.

```csharp
public int CurrentValue { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ScrollBarPropertyCurrentValueDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till ett rullningsfält i kalkylbladet
            Aspose.Cells.Drawing.ScrollBar scrollBar = (Aspose.Cells.Drawing.ScrollBar)worksheet.Shapes.AddScrollBar(1, 0, 1, 1, 100, 20);

            // Ställ in rullningsfältsegenskaper med korrekta egenskapsnamn
            scrollBar.Min = 0;
            scrollBar.Max = 100;
            scrollBar.IncrementalChange = 5;
            scrollBar.PageChange = 20;

            // Ställ in och demonstrera CurrentValue-egenskapen
            scrollBar.CurrentValue = 50;
            Console.WriteLine("ScrollBar CurrentValue: " + scrollBar.CurrentValue);

            // Ändra det aktuella värdet
            scrollBar.CurrentValue = 75;
            Console.WriteLine("Updated ScrollBar CurrentValue: " + scrollBar.CurrentValue);

            // Spara arbetsboken
            workbook.Save("ScrollBarCurrentValueDemo.xlsx");
        }
    }
}
```

### Se även

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


