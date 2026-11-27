---
title: "ScrollBar.Max"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ScrollBar property. Hämtar eller anger det maximala värdet för en rullningslist eller spinnerintervall"
type: docs
url: /sv/net/aspose.cells.drawing/scrollbar/max/
---
## ScrollBar.Max property

Hämtar eller anger det maximala värdet för ett rullningslist‑ eller spinnerintervall.

```csharp
public int Max { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ScrollBarPropertyMaxDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till ett rullningsfält i kalkylbladet
            Aspose.Cells.Drawing.ScrollBar scrollBar = (Aspose.Cells.Drawing.ScrollBar)worksheet.Shapes.AddScrollBar(1, 0, 1, 1, 100, 20);

            // Ställ in rullningsfältsegenskaper
            scrollBar.Min = 0;
            scrollBar.Max = 100; // Demonstrating Max property usage
            scrollBar.CurrentValue = 50;
            scrollBar.IncrementalChange = 5;
            scrollBar.PageChange = 10;

            // Spara arbetsboken
            workbook.Save("ScrollBarMaxDemo.xlsx");

            // Visa information
            Console.WriteLine("ScrollBar created with Max value: " + scrollBar.Max.ToString());
            Console.WriteLine("File saved successfully.");
        }
    }
}
```

### Se även

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


