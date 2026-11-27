---
title: "ScrollBar.IncrementalChange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ScrollBar property. Hämtar eller anger mängden som rullningslisten eller spinnern ökas per radrullning"
type: docs
url: /sv/net/aspose.cells.drawing/scrollbar/incrementalchange/
---
## ScrollBar.IncrementalChange property

Hämtar eller anger mängden som rullningslisten eller spinnern ökas med en radrullning.

```csharp
public int IncrementalChange { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ScrollBarPropertyIncrementalChangeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till ett rullningsfält i kalkylbladet
            ScrollBar scrollBar = worksheet.Shapes.AddScrollBar(1, 0, 1, 1, 100, 20);

            // Ställ in rullningsfältsegenskaper
            scrollBar.Min = 0;
            scrollBar.Max = 100;
            scrollBar.CurrentValue = 50;
            scrollBar.IncrementalChange = 5; // This is the key property we're demonstrating
            scrollBar.PageChange = 20;

            // Visa rullningslistens egenskaper
            Console.WriteLine("Scroll Bar Properties:");
            Console.WriteLine("Min: " + scrollBar.Min);
            Console.WriteLine("Max: " + scrollBar.Max);
            Console.WriteLine("Current Value: " + scrollBar.CurrentValue);
            Console.WriteLine("Incremental Change: " + scrollBar.IncrementalChange);
            Console.WriteLine("Page Change: " + scrollBar.PageChange);

            // Ändra den inkrementella förändringen
            scrollBar.IncrementalChange = 10;
            Console.WriteLine("\nModified Incremental Change: " + scrollBar.IncrementalChange);

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


