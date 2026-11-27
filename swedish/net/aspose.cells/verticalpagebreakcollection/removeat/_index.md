---
title: "VerticalPageBreakCollection.RemoveAt"
second_title: "Aspose.Cells för .NET API‑referens"
description: "VerticalPageBreakCollection‑metod. Tar bort VPageBreak‑elementet med ett angivet namn"
type: docs
url: /sv/net/aspose.cells/verticalpagebreakcollection/removeat/
---
## VerticalPageBreakCollection.RemoveAt method

Tar bort VPageBreak‑elementet med ett angivet namn.

```csharp
public void RemoveAt(int index)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Int32 | Elementindex, nollbaserat. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            VerticalPageBreakCollection verticalPageBreaks = worksheet.VerticalPageBreaks;

            verticalPageBreaks.Add(0, 10, 2);
            verticalPageBreaks.Add(4);
            verticalPageBreaks.Add(5, 3);
            verticalPageBreaks.Add("G5");

            verticalPageBreaks.RemoveAt(1);

            for (int i = 0; i < verticalPageBreaks.Count; i++)
            {
                VerticalPageBreak vpb = verticalPageBreaks[i];
                Console.WriteLine($"Vertical Page Break {i}: Column = {vpb.Column}, StartRow = {vpb.StartRow}, EndRow = {vpb.EndRow}");
            }

            workbook.Save("VerticalPageBreakCollectionExample.xlsx");
        }
    }
}
```

### Se även

* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


