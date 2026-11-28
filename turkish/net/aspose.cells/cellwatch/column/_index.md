---
title: "CellWatch.Column"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellWatch özelliği. Hücrenin sütununu alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/cellwatch/column/
---
## CellWatch.Column property

Hücrenin sütununu alır ve ayarlar.

```csharp
public int Column { get; set; }
```

### Örnekler

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

### Ayrıca Bakınız

* class [CellWatch](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


