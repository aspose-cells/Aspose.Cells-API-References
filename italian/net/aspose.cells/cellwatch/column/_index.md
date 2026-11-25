---
title: "CellWatch.Column"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "CellWatch proprietà. Ottiene e imposta la colonna della cella"
type: docs
url: /it/net/aspose.cells/cellwatch/column/
---
## CellWatch.Column property

Ottiene e imposta la colonna della cella.

```csharp
public int Column { get; set; }
```

### Esempi

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

### Vedi anche

* class [CellWatch](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


