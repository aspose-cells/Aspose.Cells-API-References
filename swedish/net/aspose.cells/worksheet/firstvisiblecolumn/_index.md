---
title: "Worksheet.FirstVisibleColumn"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-egenskap. Representerar index för den första synliga kolumnen"
type: docs
url: /sv/net/aspose.cells/worksheet/firstvisiblecolumn/
---
## Worksheet.FirstVisibleColumn property

Representerar första synliga kolumnens index.

```csharp
public int FirstVisibleColumn { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyFirstVisibleColumnDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Dölj den första kolumnen (index 0)
            worksheet.Cells.HideColumn(0);
            
            // Hämta och visa index för den första synliga kolumnen
            Console.WriteLine("First visible column index: " + worksheet.FirstVisibleColumn);
            
            // Spara arbetsboken
            workbook.Save("FirstVisibleColumnDemo.xlsx");
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


