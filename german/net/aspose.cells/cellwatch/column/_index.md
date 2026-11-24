---
title: "CellWatch.Column"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellWatch-Eigenschaft. Liest und schreibt die Spalte der Zelle."
type: docs
url: /de/net/aspose.cells/cellwatch/column/
---
## CellWatch.Column property

Ermittelt und setzt die Spalte der Zelle.

```csharp
public int Column { get; set; }
```

### Beispiele

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

### Siehe auch

* class [CellWatch](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


