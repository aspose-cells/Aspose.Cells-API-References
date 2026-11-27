---
title: "Worksheet.IsPageBreakPreview"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-egenskap. Anger om det angivna kalkylbladet visas i normal vy eller sidbrytning‑förhandsgranskning"
type: docs
url: /sv/net/aspose.cells/worksheet/ispagebreakpreview/
---
## Worksheet.IsPageBreakPreview property

Anger om det angivna kalkylbladet visas i normal vy eller sidbrytning förhandsgranskning.

```csharp
public bool IsPageBreakPreview { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsPageBreakPreviewDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in kalkylbladet i Page Break Preview‑läge
            worksheet.IsPageBreakPreview = true;
            
            // Ställ in zoom till 100 % för demonstration
            worksheet.Zoom = 100;
            
            // Skriv ut de aktuella inställningarna
            Console.WriteLine("IsPageBreakPreview: " + worksheet.IsPageBreakPreview);
            Console.WriteLine("Zoom: " + worksheet.Zoom);
            
            // Spara arbetsboken
            workbook.Save("WorksheetPropertyIsPageBreakPreviewDemo_output.xlsx");
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


