---
title: "Cell.ContainsExternalLink"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-egenskap. Anger om denna cell innehåller en extern länk. Gäller endast när cellen är en formelcell"
type: docs
url: /sv/net/aspose.cells/cell/containsexternallink/
---
## Cell.ContainsExternalLink property

Anger om den här cellen innehåller en extern länk. Gäller endast när cellen är en formelcell.

```csharp
public bool ContainsExternalLink { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyContainsExternalLinkDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet sheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata och extern länk
            sheet.Cells["A1"].PutValue("External Link:");
            sheet.Cells["B1"].Formula = "=HYPERLINK(\"https://www.aspose.com\", \"Aspose\")";
            
            // Kontrollera om celler innehåller externa länkar
            Console.WriteLine("A1 ContainsExternalLink: " + sheet.Cells["A1"].ContainsExternalLink);
            Console.WriteLine("B1 ContainsExternalLink: " + sheet.Cells["B1"].ContainsExternalLink);
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


