---
title: "Range.UnionRanges"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Range. تُرجع نتيجة الاتحاد لنطاقين"
type: docs
url: /ar/net/aspose.cells/range/unionranges/
---
## Range.UnionRanges method

يرجع نتيجة اتحاد نطاقين.

```csharp
public UnionRange UnionRanges(Range[] ranges)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| نطاقات | Range[] | النطاق |

### قيمة الإرجاع

الاتحاد بين نطاقين.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangeMethodUnionRangesWithRangeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء بيانات عينة في الخلايا
            worksheet.Cells["A1"].PutValue("Range 1");
            worksheet.Cells["B1"].PutValue("Data 1");
            worksheet.Cells["C1"].PutValue("Data 2");
            worksheet.Cells["A5"].PutValue("Range 2");
            worksheet.Cells["B5"].PutValue("Data 3");
            worksheet.Cells["C5"].PutValue("Data 4");

            // إنشاء نطاقات للدمج
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:C3");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("A5:C7");

            try
            {
                // استدعاء UnionRanges مع معامل Range[]
                Aspose.Cells.Range[] rangesToUnion = new Aspose.Cells.Range[] { range1, range2 };
                UnionRange unionRange = range1.UnionRanges(rangesToUnion);

                // تطبيق نمط لإظهار النطاق المدمج
                Style style = workbook.CreateStyle();
                style.BackgroundColor = System.Drawing.Color.LightBlue;
                unionRange.ApplyStyle(style, new StyleFlag { All = true });

                Console.WriteLine($"Union range created successfully. Address: {unionRange.RefersTo}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UnionRanges method: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("UnionRangesDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [UnionRange](../../unionrange/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


