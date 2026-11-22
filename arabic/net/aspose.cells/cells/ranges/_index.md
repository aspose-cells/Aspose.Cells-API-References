---
title: "Cells.Ranges"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cells. تحصل على مجموعة كائنات Range التي تم إنشاؤها أثناء التشغيل"
type: docs
url: /ar/net/aspose.cells/cells/ranges/
---
## Cells.Ranges property

يحصل على مجموعة كائنات [`Range`](../../range/) التي تم إنشاؤها أثناء التشغيل.

```csharp
public RangeCollection Ranges { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyRangesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أنشئ وأضف نطاقًا إلى مجموعة Ranges
            Aspose.Cells.Range cellRange = worksheet.Cells.CreateRange(0, 0, 3, 1);
            worksheet.Cells.Ranges.Add(cellRange);
            
            // أدرج صفوفًا وأظهر توسع النطاق
            worksheet.Cells.InsertRows(2, 2, true);
            
            Console.WriteLine($"Range row count after insertion: {cellRange.RowCount}");
        }
    }
}
```

### انظر أيضًا

* class [RangeCollection](../../rangecollection/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


