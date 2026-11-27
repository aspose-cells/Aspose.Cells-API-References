---
title: "HorizontalPageBreak.EndColumn"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HorizontalPageBreak property. Hämtar slutkolumnens index för denna horisontella sidbrytning"
type: docs
url: /sv/net/aspose.cells/horizontalpagebreak/endcolumn/
---
## HorizontalPageBreak.EndColumn property

Hämtar slutkolumnindex för detta horisontella sidbrytning.

```csharp
public int EndColumn { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakPropertyEndColumnDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en horisontell sidbrytning på rad 5, som sträcker sig från kolumn 2 till 4
            int index = worksheet.HorizontalPageBreaks.Add(5, 2, 4);
            HorizontalPageBreak hPageBreak = worksheet.HorizontalPageBreaks[index];

            // Visa EndColumn-egenskapen
            Console.WriteLine("Horizontal Page Break EndColumn: " + hPageBreak.EndColumn);

            // Eftersom EndColumn är skrivskyddad måste vi ta bort och återlägga sidbrytningen för att ändra den
            worksheet.HorizontalPageBreaks.RemoveAt(index);
            index = worksheet.HorizontalPageBreaks.Add(5, 2, 6);
            hPageBreak = worksheet.HorizontalPageBreaks[index];
            Console.WriteLine("Modified Horizontal Page Break EndColumn: " + hPageBreak.EndColumn);
        }
    }
}
```

### Se även

* class [HorizontalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


