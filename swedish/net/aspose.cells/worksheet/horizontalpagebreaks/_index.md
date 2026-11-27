---
title: "Worksheet.HorizontalPageBreaks"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet egenskap. Hämtar HorizontalPageBreakCollection-samlingen"
type: docs
url: /sv/net/aspose.cells/worksheet/horizontalpagebreaks/
---
## Worksheet.HorizontalPageBreaks property

Hämtar [`HorizontalPageBreakCollection`](../../horizontalpagebreakcollection/) samlingen.

```csharp
public HorizontalPageBreakCollection HorizontalPageBreaks { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyHorizontalPageBreaksDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till horisontella sidbrytningar på olika sätt
            worksheet.HorizontalPageBreaks.Add(5);
            worksheet.HorizontalPageBreaks.Add(10, 1, 5);
            worksheet.HorizontalPageBreaks.Add(15, 2);
            worksheet.HorizontalPageBreaks.Add("G5");

            // Ta bort den första sidbrytningen
            worksheet.HorizontalPageBreaks.RemoveAt(0);

            // Spara utdata
            workbook.Save("HorizontalPageBreaksDemo.xlsx");
            workbook.Save("HorizontalPageBreaksDemo.pdf");
        }
    }
}
```

### Se även

* class [HorizontalPageBreakCollection](../../horizontalpagebreakcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


