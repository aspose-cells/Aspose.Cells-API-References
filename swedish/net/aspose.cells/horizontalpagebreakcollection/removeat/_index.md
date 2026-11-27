---
title: "HorizontalPageBreakCollection.RemoveAt"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HorizontalPageBreakCollection-metod. Tar bort HPageBreak-elementet med ett angivet namn"
type: docs
url: /sv/net/aspose.cells/horizontalpagebreakcollection/removeat/
---
## HorizontalPageBreakCollection.RemoveAt method

Tar bort HPageBreak-elementet med ett angivet namn.

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
    public class HorizontalPageBreakCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.HorizontalPageBreaks.Add(5);
            worksheet.HorizontalPageBreaks.Add(10);
            worksheet.HorizontalPageBreaks.Add(15);
            
            worksheet.HorizontalPageBreaks.RemoveAt(0);
            
            workbook.Save("HorizontalPageBreakCollectionExample.xlsx");
        }
    }
}
```

### Se även

* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


