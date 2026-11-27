---
title: "Range.UnMerge"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range-metod. Avslår sammanslagna celler i detta område"
type: docs
url: /sv/net/aspose.cells/range/unmerge/
---
## Range.UnMerge method

Avslår sammanslagna celler i detta område.

```csharp
public void UnMerge()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodUnMergeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Sammanfoga celler B2 till D4
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2", "D4");
            range.Merge();
            
            // Kontrollera om cell B2 är sammanslagen innan den avsammanfogas
            Console.WriteLine("Before UnMerge - Is B2 merged? " + worksheet.Cells["B2"].IsMerged);
            
            // Avsammanfoga området
            range.UnMerge();
            
            // Kontrollera om cell B2 är sammanslagen efter avsammanfogning
            Console.WriteLine("After UnMerge - Is B2 merged? " + worksheet.Cells["B2"].IsMerged);
        }
    }
}
```

### Se även

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


