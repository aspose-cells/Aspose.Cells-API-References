---
title: "RangeCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة RangeCollection. يضيف عنصر Range إلى المجموعة"
type: docs
url: /ar/net/aspose.cells/rangecollection/add/
---
## RangeCollection.Add method

يضيف عنصر [`Range`](../../range/) إلى المجموعة.

```csharp
[Obsolete("Use RangeCollection.AddRange(Range) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(Range range)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| نطاق | النطاق | كائن Range |

### ملاحظات

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام طريقة AddRange(). سيتم إزالة هذه الطريقة بعد 6 أشهر منذ ديسمبر 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeCollectionMethodAddWithRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء نطاق وإضافته إلى المجموعة
            Aspose.Cells.Range cellRange = worksheet.Cells.CreateRange(0, 0, 3, 1);
            worksheet.Cells.Ranges.Add(cellRange);
            
            // إدراج صفوف لعرض توسع النطاق
            worksheet.Cells.InsertRows(2, 2);
            
            Console.WriteLine("Range row count after insertion: " + cellRange.RowCount);
        }
    }
}
```

### انظر أيضًا

* class [Range](../../range/)
* class [RangeCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


