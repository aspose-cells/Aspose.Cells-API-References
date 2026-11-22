---
title: "Range.UnionRang"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Range. تُرجع نتيجة الاتحاد لنطاقين"
type: docs
url: /ar/net/aspose.cells/range/unionrang/
---
## Range.UnionRang method

يرجع نتيجة اتحاد نطاقين.

```csharp
[Obsolete("Use Range.UnionRanges() instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public Range[] UnionRang(Range range)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| نطاق | النطاق | النطاق |

### قيمة الإرجاع

الاتحاد بين نطاقين.

### ملاحظات

ملاحظة: هذه الطريقة الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة Range.UnionRanges(). سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ مايو 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using Range = Aspose.Cells.Range; // Add this alias to resolve ambiguity

    public class RangeMethodUnionRangWithRangeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء نطاقين لتوضيح UnionRang
            Range range1 = worksheet.Cells.CreateRange("A1:B2");
            Range range2 = worksheet.Cells.CreateRange("C3:D4");

            // تعيين بعض القيم في النطاقات للتصوير
            range1[0, 0].PutValue("Range1");
            range1[1, 1].PutValue("Data");
            range2[0, 0].PutValue("Range2");
            range2[1, 1].PutValue("Data");

            try
            {
                // استدعاء طريقة UnionRang لدمج النطاقين
                Range[] unionResult = range1.UnionRang(range2);

                // عرض معلومات حول نتيجة الاتحاد
                Console.WriteLine("UnionRang method executed successfully.");
                Console.WriteLine($"Number of ranges in union: {unionResult.Length}");
                Console.WriteLine($"First union range address: {unionResult[0].Address}");
                Console.WriteLine($"Second union range address: {unionResult[1].Address}");

                // تمييز نطاقات الاتحاد بحدود للتصوير
                foreach (Range r in unionResult)
                {
                    r.SetOutlineBorders(CellBorderType.Thin, System.Drawing.Color.Black);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UnionRang method: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("RangeMethodUnionRangWithRangeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


