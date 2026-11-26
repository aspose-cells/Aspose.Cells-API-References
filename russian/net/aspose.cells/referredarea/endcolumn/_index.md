---
title: "ReferredArea.EndColumn"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ReferredArea. Конечный столбец области"
type: docs
url: /ru/net/aspose.cells/referredarea/endcolumn/
---
## ReferredArea.EndColumn property

Конечный столбец области.

```csharp
public int EndColumn { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReferredAreaPropertyEndColumnDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            Cell cell = worksheet.Cells["B2"];
            cell.Formula = "=SUM(A1:C3)";
            
            ReferredAreaCollection referredAreas = cell.GetPrecedents();
            foreach (ReferredArea area in referredAreas)
            {
                Console.WriteLine($"StartColumn: {area.StartColumn}");
                Console.WriteLine($"EndColumn: {area.EndColumn}");
                Console.WriteLine($"Columns spanned: {area.EndColumn - area.StartColumn + 1}");
            }
        }
    }
}
```

### См. также

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


