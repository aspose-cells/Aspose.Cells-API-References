---
title: "Worksheet.RemoveSplit"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet method. Tar bort delningsfönstret"
type: docs
url: /sv/net/aspose.cells/worksheet/removesplit/
---
## Worksheet.RemoveSplit method

Tar bort delat fönster.

```csharp
public void RemoveSplit()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodRemoveSplitDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Dela worksheet
            worksheet.Split();
            Console.WriteLine("Worksheet split state: " + worksheet.PaneState);
            
            // Ta bort delningen
            worksheet.RemoveSplit();
            Console.WriteLine("Worksheet split state after RemoveSplit: " + worksheet.PaneState);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


