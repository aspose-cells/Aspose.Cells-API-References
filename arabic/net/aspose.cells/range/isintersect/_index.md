---
title: "Range.IsIntersect"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Range. تشير إلى ما إذا كان النطاق يتقاطع"
type: docs
url: /ar/net/aspose.cells/range/isintersect/
---
## Range.IsIntersect method

يشير إلى ما إذا كان النطاق متقاطعًا.

```csharp
public bool IsIntersect(Range range)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| نطاق | النطاق | النطاق. |

### قيمة الإرجاع

ما إذا كان النطاق يتقاطع.

### ملاحظات

إذا لم تكن النطاقان في نفس ورقة العمل، تُرجع false.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangeMethodIsIntersectWithRangeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء نطاقين لاختبار التقاطع
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B5");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("B3:D8");
            Aspose.Cells.Range range3 = worksheet.Cells.CreateRange("C10:D15");

            try
            {
                // تحقق مما إذا كان range1 يتقاطع مع range2 (يجب أن يتقاطع)
                bool result1 = range1.IsIntersect(range2);
                Console.WriteLine($"Range A1:B5 intersects with B3:D8: {result1}");

                // تحقق مما إذا كان range1 يتقاطع مع range3 (يجب ألا يتقاطع)
                bool result2 = range1.IsIntersect(range3);
                Console.WriteLine($"Range A1:B5 intersects with C10:D15: {result2}");

                // ملء النطاقات بألوان مختلفة لتصويرها
                Style style1 = workbook.CreateStyle();
                style1.ForegroundColor = System.Drawing.Color.LightBlue;
                style1.Pattern = BackgroundType.Solid;
                range1.SetStyle(style1);

                Style style2 = workbook.CreateStyle();
                style2.ForegroundColor = System.Drawing.Color.LightGreen;
                style2.Pattern = BackgroundType.Solid;
                range2.SetStyle(style2);

                Style style3 = workbook.CreateStyle();
                style3.ForegroundColor = System.Drawing.Color.LightPink;
                style3.Pattern = BackgroundType.Solid;
                range3.SetStyle(style3);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IsIntersect method: {ex.Message}");
            }

            // احفظ المصنف
            workbook.Save("RangeMethodIsIntersectWithRangeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


