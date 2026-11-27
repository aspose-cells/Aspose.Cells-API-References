---
title: "Outline.SummaryColumnRight"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Outline-egenskap. Anger om sammanfattningskolumnen ska placeras till höger om detaljkollumnerna i dispositionen"
type: docs
url: /sv/net/aspose.cells/outline/summarycolumnright/
---
## Outline.SummaryColumnRight property

Anger om sammanfattningskolumnen kommer att placeras till höger om detaljkolumnerna i konturen.

```csharp
public bool SummaryColumnRight { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OutlinePropertySummaryColumnRightDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata och gruppera rader
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue("Item " + (i + 1));
                worksheet.Cells["B" + (i + 1)].PutValue(i * 10);
            }

            // Gruppera rader (skapar en disposition)
            worksheet.Cells.GroupRows(0, 9, false);

            // Hämta dispositionens inställningar
            Outline outline = worksheet.Outline;

            // Ställ in SummaryColumnRight till true (sammanfattningskolumner visas till höger om detaljkollumnerna)
            outline.SummaryColumnRight = true;
            Console.WriteLine("SummaryColumnRight is set to: " + outline.SummaryColumnRight);

            // Spara arbetsboken
            workbook.Save("OutlinePropertySummaryColumnRightDemo.xlsx");
        }
    }
}
```

### Se även

* class [Outline](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


