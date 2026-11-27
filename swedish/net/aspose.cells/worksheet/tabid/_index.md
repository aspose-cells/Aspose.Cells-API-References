---
title: "Worksheet.TabId"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet property. Anger det interna identifieraren för bladet"
type: docs
url: /sv/net/aspose.cells/worksheet/tabid/
---
## Worksheet.TabId property

Anger den interna identifieraren för bladet.

```csharp
public int TabId { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTabIdDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in TabId-egenskapen
            worksheet.TabId = 107;
            
            // Spara arbetsboken
            string outputPath = "output.xlsb";
            workbook.Save(outputPath);
            
            // Läs in den sparade workbook för att verifiera TabId
            Workbook loadedWorkbook = new Workbook(outputPath);
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            
            // Visa TabId-värdet
            Console.WriteLine("Worksheet TabId: " + loadedWorksheet.TabId);
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


