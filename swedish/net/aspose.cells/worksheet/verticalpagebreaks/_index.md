---
title: "Worksheet.VerticalPageBreaks"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-egenskap. Hämtar VerticalPageBreakCollection-samlingen"
type: docs
url: /sv/net/aspose.cells/worksheet/verticalpagebreaks/
---
## Worksheet.VerticalPageBreaks property

Hämtar [`VerticalPageBreakCollection`](../../verticalpagebreakcollection/) samlingen.

```csharp
public VerticalPageBreakCollection VerticalPageBreaks { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyVerticalPageBreaksDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            VerticalPageBreakCollection verticalPageBreaks = worksheet.VerticalPageBreaks;

            // Lägg till olika typer av vertikala sidbrytningar
            verticalPageBreaks.Add(0, 10, 2);
            verticalPageBreaks.Add(4);
            verticalPageBreaks.Add(5, 3);
            verticalPageBreaks.Add("G5");

            // Ta bort en sidbrytning
            verticalPageBreaks.RemoveAt(1);

            // Skriv ut information om sidbrytning
            for (int i = 0; i < verticalPageBreaks.Count; i++)
            {
                VerticalPageBreak vpb = verticalPageBreaks[i];
                Console.WriteLine($"Break {i}: StartRow={vpb.StartRow}, EndRow={vpb.EndRow}, Column={vpb.Column}");
            }

            workbook.Save("VerticalPageBreaksDemo.xlsx");
        }
    }
}
```

### Se även

* class [VerticalPageBreakCollection](../../verticalpagebreakcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


