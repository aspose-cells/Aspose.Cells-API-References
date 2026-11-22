---
title: "CellWatch.Column"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CellWatch. تحصل وتعيّن عمود الخلية"
type: docs
url: /ar/net/aspose.cells/cellwatch/column/
---
## CellWatch.Column property

يحصل على عمود الخلية ويضبطه.

```csharp
public int Column { get; set; }
```

### أمثلة

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

### انظر أيضًا

* class [CellWatch](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


