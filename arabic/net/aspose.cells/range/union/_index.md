---
title: "Range.Union"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Range. إرجاع اتحاد نطاقين"
type: docs
url: /ar/net/aspose.cells/range/union/
---
## Range.Union method

يرجع اتحاد نطاقين.

```csharp
[Obsolete("Use Range.UnionRanges() instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList Union(Range range)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| نطاق | النطاق | النطاق |

### قيمة الإرجاع

الاتحاد بين نطاقين.

### ملاحظات

ملاحظة: هذه الطريقة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة Range.UnionRanges(). سيتم إزالة هذه الطريقة بعد 12 شهرًا اعتبارًا من نوفمبر 2023. شركة Aspose تعتذر عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class RangeMethodUnionWithRangeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء نطاقين لتوضيح الاتحاد
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B2");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("B2:C3");

            // ملء بعض البيانات في النطاقات
            range1[0, 0].PutValue("Range1");
            range2[0, 0].PutValue("Range2");

            try
            {
                // استدعاء طريقة Union (ملاحظة: هذه هي النسخة المهجورة)
                ArrayList unionResult = range1.Union(range2);

                Console.WriteLine("Union method executed successfully");
                Console.WriteLine($"Number of ranges in union: {unionResult.Count}");

                // عرض عناوين جميع النطاقات في الاتحاد
                foreach (Aspose.Cells.Range r in unionResult)
                {
                    Console.WriteLine($"Union range address: {r.Address}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Union method: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("RangeMethodUnionWithRangeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


