---
title: "Worksheet.AddPageBreaks"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet metod. Lägger till sidbrytning"
type: docs
url: /sv/net/aspose.cells/worksheet/addpagebreaks/
---
## Worksheet.AddPageBreaks method

Lägger till sidbrytning.

```csharp
public void AddPageBreaks(string cellName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellName | String |  |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAddPageBreaksWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till horisontell sidbrytning på rad 1 (B2)
            worksheet.AddPageBreaks("B2");

            // Lägg till horisontell sidbrytning på rad 9 (B10)
            worksheet.AddPageBreaks("B10");

            // Verifiera att den första sidbrytningen lades till på rad 1
            Console.WriteLine("First page break row: " + worksheet.HorizontalPageBreaks[0].Row);
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


