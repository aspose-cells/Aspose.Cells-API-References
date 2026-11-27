---
title: "HorizontalPageBreak.StartColumn"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HorizontalPageBreak‑egenskap. Hämtar startkolumnindex för detta horisontella sidbrytning"
type: docs
url: /sv/net/aspose.cells/horizontalpagebreak/startcolumn/
---
## HorizontalPageBreak.StartColumn property

Hämtar startkolumnindex för detta horisontella sidbrytning.

```csharp
public int StartColumn { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakPropertyStartColumnDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till sidbrytningar i olika kolumner för att demonstrera StartColumn
            int index1 = worksheet.HorizontalPageBreaks.Add("Y30");
            int index2 = worksheet.HorizontalPageBreaks.Add("B30");
            
            HorizontalPageBreak hPageBreak1 = worksheet.HorizontalPageBreaks[index1];
            HorizontalPageBreak hPageBreak2 = worksheet.HorizontalPageBreaks[index2];
            
            Console.WriteLine($"First Break Start Column: {hPageBreak1.StartColumn}");
            Console.WriteLine($"Second Break Start Column: {hPageBreak2.StartColumn}");
            
            workbook.Save("HorizontalPageBreakExample.xlsx");
        }
    }
}
```

### Se även

* class [HorizontalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


