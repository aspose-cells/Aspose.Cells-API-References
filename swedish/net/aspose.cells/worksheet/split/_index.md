---
title: "Worksheet.Split"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet‑metod. Delar fönstret"
type: docs
url: /sv/net/aspose.cells/worksheet/split/
---
## Worksheet.Split method

Delar fönster.

```csharp
public void Split()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodSplitDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för att demonstrera delning
            worksheet.Cells["A1"].PutValue("Header");
            for (int i = 1; i <= 50; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue("Data " + i);
            }
            
            // Dela kalkylbladet (inga parametrar behövs)
            worksheet.Split();
            
            // Spara arbetsboken
            workbook.Save("WorksheetSplitDemo.xml", SaveFormat.SpreadsheetML);
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


