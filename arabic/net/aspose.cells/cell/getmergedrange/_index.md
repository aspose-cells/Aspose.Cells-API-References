---
title: "Cell.GetMergedRange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cell. تُعيد كائن Range الذي يمثل نطاقًا مدموجًا"
type: docs
url: /ar/net/aspose.cells/cell/getmergedrange/
---
## Cell.GetMergedRange method

تُعيد كائن [`Range`](../../range/) الذي يمثل نطاقًا مدموجًا.

```csharp
public Range GetMergedRange()
```

### قيمة الإرجاع

[`Range`](../../range/) object. Null if this cell is not merged.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetMergedRangeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // دمج الخلايا
            cells.Merge(0, 0, 2, 2);

            // احصل على الخلية الأولى
            Cell cell = cells[0, 0];

            // احصل على معلومات النطاق المدموج
            Aspose.Cells.Range mergedRange = cell.GetMergedRange();
            
            // أخرج تفاصيل النطاق المدموج
            Console.WriteLine("Merged Range Details:");
            Console.WriteLine($"First Row: {mergedRange.FirstRow}");
            Console.WriteLine($"First Column: {mergedRange.FirstColumn}");
            Console.WriteLine($"Row Count: {mergedRange.RowCount}");
            Console.WriteLine($"Column Count: {mergedRange.ColumnCount}");
        }
    }
}
```

### انظر أيضًا

* class [Range](../../range/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


