---
title: "ScrollBar.PageChange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ScrollBar property. Hämtar eller anger sidändring"
type: docs
url: /sv/net/aspose.cells.drawing/scrollbar/pagechange/
---
## ScrollBar.PageChange property

Hämtar eller anger sidbyte

```csharp
public int PageChange { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ScrollBarPropertyPageChangeDemo
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
            scrollBar.IncrementalChange = 1;
            scrollBar.PageChange = 10; // Demonstrate PageChange property
            scrollBar.LinkedCell = "A1";

            // Spara arbetsboken
            workbook.Save("ScrollBarPropertyPageChangeDemo.xlsx");

            // Läs in den sparade arbetsboken för att verifiera egenskaperna
            Workbook verifyWorkbook = new Workbook("ScrollBarPropertyPageChangeDemo.xlsx");
            ScrollBar verifyScrollBar = (ScrollBar)verifyWorkbook.Worksheets[0].Shapes[0];

            // Skriv ut värdet för PageChange-egenskapen för att demonstrera att det sparades/laddades korrekt
            Console.WriteLine("ScrollBar PageChange value: " + verifyScrollBar.PageChange);
        }
    }
}
```

### Se även

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


