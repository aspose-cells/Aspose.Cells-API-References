---
title: "Cell.IsMerged"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cell. تتحقق مما إذا كانت الخلية جزءًا من نطاق مدمج أم لا"
type: docs
url: /ar/net/aspose.cells/cell/ismerged/
---
## Cell.IsMerged property

يتحقق مما إذا كانت الخلية جزءًا من نطاق مدمج أم لا.

```csharp
public bool IsMerged { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsMergedDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // دمج الخلايا من A1 إلى B2
            worksheet.Cells.Merge(0, 0, 2, 2);

            // تحقق مما إذا كانت الخلية A1 مدمجة
            bool isMerged = worksheet.Cells["A1"].IsMerged;
            Console.WriteLine("Is cell A1 merged? " + isMerged);

            // تحقق مما إذا كانت الخلية C1 مدمجة (يجب أن تكون خاطئة)
            isMerged = worksheet.Cells["C1"].IsMerged;
            Console.WriteLine("Is cell C1 merged? " + isMerged);

            // احفظ المصنف
            workbook.Save("MergedCellsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


