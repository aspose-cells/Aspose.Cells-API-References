---
title: "Klass VerticalPageBreak"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.VerticalPageBreak klass. Inkapslar objektet som representerar en vertikal sidbrytning"
type: docs
url: /sv/net/aspose.cells/verticalpagebreak/
---
## VerticalPageBreak class

Inkapslar objektet som representerar ett vertikalt sidbryt.

```csharp
public class VerticalPageBreak
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Column](../../aspose.cells/verticalpagebreak/column/) { get; } | Hämtar kolumnindexet för den vertikala sidbrytningen. |
| [EndRow](../../aspose.cells/verticalpagebreak/endrow/) { get; } | Hämtar slutradens index för den vertikala sidbrytningen. |
| [StartRow](../../aspose.cells/verticalpagebreak/startrow/) { get; } | Hämtar startradens index för den vertikala sidbrytningen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class VerticalPageBreakDemo
    {
        public static void VerticalPageBreakExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en vertikal sidbrytning i kolumn G (index 6)
            worksheet.VerticalPageBreaks.Add("G5");

            // Spara arbetsboken
            workbook.Save("VerticalPageBreakExample.xlsx");

            // Åtkomst till den tillagda vertikala sidbrytningen
            VerticalPageBreak vpb = worksheet.VerticalPageBreaks[0];

            // Visa egenskaperna för den vertikala sidbrytningen
            Console.WriteLine("Start Row: " + vpb.StartRow);
            Console.WriteLine("End Row: " + vpb.EndRow);
            Console.WriteLine("Column: " + vpb.Column);
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


