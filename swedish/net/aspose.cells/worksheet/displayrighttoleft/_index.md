---
title: "Worksheet.DisplayRightToLeft"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet‑egenskap. Anger om det angivna kalkylbladet visas från höger till vänster istället för från vänster till höger. Standard är falskt"
type: docs
url: /sv/net/aspose.cells/worksheet/displayrighttoleft/
---
## Worksheet.DisplayRightToLeft property

Anger om det angivna kalkylbladet visas från höger till vänster istället för från vänster till höger. Standard är falskt.

```csharp
public bool DisplayRightToLeft { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyDisplayRightToLeftDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in visning från höger till vänster
            worksheet.DisplayRightToLeft = true;
            
            // Spara arbetsboken
            workbook.Save("output.ods");
            
            // Ladda om arbetsboken för att verifiera inställningen
            Workbook loadedWorkbook = new Workbook("output.ods");
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            
            Console.WriteLine("DisplayRightToLeft: " + loadedWorksheet.DisplayRightToLeft);
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


