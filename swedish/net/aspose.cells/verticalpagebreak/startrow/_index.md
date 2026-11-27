---
title: "VerticalPageBreak.StartRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "VerticalPageBreak-egenskap. Hämtar startradens index för den vertikala sidbrytningen"
type: docs
url: /sv/net/aspose.cells/verticalpagebreak/startrow/
---
## VerticalPageBreak.StartRow property

Hämtar startradens index för den vertikala sidbrytningen.

```csharp
public int StartRow { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakPropertyStartRowDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till vertikala sidbrytningar med önskad startrad (2) initialt
            worksheet.VerticalPageBreaks.Add(2, 0, 10);
            VerticalPageBreak vPageBreak = worksheet.VerticalPageBreaks[0];

            // Visa StartRow-egenskapen
            Console.WriteLine("Vertical Page Break Start Row: " + vPageBreak.StartRow);

            // Eftersom StartRow är skrivskyddad måste vi ta bort och lägga till igen för att ändra den
            worksheet.VerticalPageBreaks.RemoveAt(0);
            worksheet.VerticalPageBreaks.Add(5, 0, 10);
            vPageBreak = worksheet.VerticalPageBreaks[0];
            Console.WriteLine("Modified Vertical Page Break Start Row: " + vPageBreak.StartRow);

            // Spara arbetsboken
            workbook.Save("VerticalPageBreakExample.xlsx");
        }
    }
}
```

### Se även

* class [VerticalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


