---
title: "Klass Outline"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Outline-klass. Representerar en kontur på ett kalkylblad"
type: docs
url: /sv/net/aspose.cells/outline/
---
## Outline class

Representerar en kontur på ett arbetsblad.

```csharp
public class Outline
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [SummaryColumnRight](../../aspose.cells/outline/summarycolumnright/) { get; set; } | Anger om sammanfattningskolumnen kommer att placeras till höger om detaljkolumnerna i konturen. |
| [SummaryRowBelow](../../aspose.cells/outline/summaryrowbelow/) { get; set; } | Anger om sammanfattningsraden kommer att placeras under detaljraderna i konturen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OutlineDemo
    {
        public static void OutlineExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Åtkomst till konturen på kalkylbladet
            Outline outline = worksheet.Outline;
            
            // Ange egenskaperna för konturen
            outline.SummaryRowBelow = true; // Indicates if the summary row will be positioned below the detail rows
            outline.SummaryColumnRight = true; // Indicates if the summary column will be positioned to the right of the detail columns
            
            // Spara arbetsboken
            workbook.Save("OutlineExample.xlsx");

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


