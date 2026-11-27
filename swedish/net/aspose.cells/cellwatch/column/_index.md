---
title: "CellWatch.Column"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellWatch-egenskap. Hämtar och anger kolumnen för cellen"
type: docs
url: /sv/net/aspose.cells/cellwatch/column/
---
## CellWatch.Column property

Hämtar och anger kolumnen för cellen.

```csharp
public int Column { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellWatchPropertyColumnDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            int watchIndex = sheet.CellWatches.Add("B2");
            CellWatch cellWatch = sheet.CellWatches[watchIndex];
            
            Console.WriteLine("Initial Column: " + cellWatch.Column);
            
            cellWatch.Column = 1;
            Console.WriteLine("Modified Column: " + cellWatch.Column);
            
            workbook.Save("CellWatchColumnDemo.xlsx");
        }
    }
}
```

### Se även

* class [CellWatch](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


