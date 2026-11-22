---
title: "ReferredArea.EndColumn"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ReferredArea. العمود النهائي للمنطقة"
type: docs
url: /ar/net/aspose.cells/referredarea/endcolumn/
---
## ReferredArea.EndColumn property

عمود النهاية للمنطقة.

```csharp
public int EndColumn { get; }
```

### أمثلة

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

### انظر أيضًا

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


