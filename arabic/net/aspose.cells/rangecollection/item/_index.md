---
title: "RangeCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RangeCollection. يحصل على عنصر Range في الفهرس المحدد"
type: docs
url: /ar/net/aspose.cells/rangecollection/item/
---
## RangeCollection indexer

يحصل على عنصر [`Range`](../../range/) في الفهرس المحدد.

```csharp
public Range this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس الذي يبدأ من الصفر للعنصر. |

### قيمة الإرجاع

العنصر عند الفهرس المحدد.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء بعض النطاقات
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B2");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("C3:D4");
            Aspose.Cells.Range range3 = worksheet.Cells.CreateRange("E5:F6");

            // أضف النطاقات إلى المجموعة
            RangeCollection ranges = worksheet.Cells.Ranges;
            ranges.Add(range1);
            ranges.Add(range2);
            ranges.Add(range3);

            // عرض استخدام خاصية Item
            Console.WriteLine("Range Collection Count: " + ranges.Count);
            for (int i = 0; i < ranges.Count; i++)
            {
                Aspose.Cells.Range currentRange = ranges[i]; // Using Item property
                Console.WriteLine($"Range {i + 1}: {currentRange.Address}");
                Console.WriteLine($"  - FirstRow: {currentRange.FirstRow}");
                Console.WriteLine($"  - FirstColumn: {currentRange.FirstColumn}");
                Console.WriteLine($"  - RowCount: {currentRange.RowCount}");
                Console.WriteLine($"  - ColumnCount: {currentRange.ColumnCount}");
            }

            // الوصول إلى نطاق محدد عبر الفهرس
            Aspose.Cells.Range secondRange = ranges[1]; // Using Item property
            Console.WriteLine("\nSecond range details:");
            Console.WriteLine($"Address: {secondRange.Address}");
        }
    }
}
```

### انظر أيضًا

* class [Range](../../range/)
* class [RangeCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


