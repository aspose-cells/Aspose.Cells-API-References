---
title: "UnionRange.Intersect"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة UnionRange. تتقاطع مع نطاق آخر"
type: docs
url: /ar/net/aspose.cells/unionrange/intersect/
---
## Intersect(string) {#intersect_2}

يتقاطع مع نطاق آخر.

```csharp
public UnionRange Intersect(string range)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| نطاق | String | النطاق. |

### ملاحظات

إذا لم تتقاطع نطاقات الاتحاد الاثنين، تُعيد null.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodIntersectWithStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // املأ بعض بيانات العينة
            worksheet.Cells["A1"].PutValue("A1");
            worksheet.Cells["B1"].PutValue("B1");
            worksheet.Cells["A2"].PutValue("A2");
            worksheet.Cells["B2"].PutValue("B2");

            // إنشاء UnionRange يغطي A1:B2
            UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });

            try
            {
                // استدعاء Intersect مع معامل سلسلة يمثل النطاق A1:A2
                UnionRange intersectionResult = unionRange.Intersect("A1:A2");

                // عرض معلومات حول التقاطع
                Console.WriteLine($"Intersection result range: {intersectionResult.RefersTo}");
                Console.WriteLine($"First row: {intersectionResult.FirstRow}");
                Console.WriteLine($"First column: {intersectionResult.FirstColumn}");
                Console.WriteLine($"Row count: {intersectionResult.RowCount}");
                Console.WriteLine($"Column count: {intersectionResult.ColumnCount}");

                // تمييز منطقة التقاطع
                Style highlightStyle = workbook.CreateStyle();
                highlightStyle.BackgroundColor = System.Drawing.Color.LightGreen;
                intersectionResult.SetStyle(highlightStyle);

                Console.WriteLine("Intersect method executed successfully with parameter (String)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Intersect method: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("UnionRangeMethodIntersectWithStringDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Intersect(UnionRange) {#intersect_1}

يتقاطع مع نطاق آخر.

```csharp
public UnionRange Intersect(UnionRange unionRange)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| unionRange | UnionRange | النطاق. |

### ملاحظات

إذا لم تتقاطع نطاقات الاتحاد الاثنين، تُعيد null.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodIntersectWithUnionRangeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ملء بعض البيانات في الخلايا
            worksheet.Cells["A1"].PutValue("A1");
            worksheet.Cells["B1"].PutValue("B1");
            worksheet.Cells["C1"].PutValue("C1");
            worksheet.Cells["A2"].PutValue("A2");
            worksheet.Cells["B2"].PutValue("B2");
            worksheet.Cells["C2"].PutValue("C2");

            // إنشاء نطاقين اتحاد
            UnionRange range1 = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });
            UnionRange range2 = worksheet.Cells.CreateRange("B1:C2").UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("B1:C2") });

            try
            {
                // استدعاء طريقة Intersect مع معامل UnionRange
                UnionRange intersectionResult = range1.Intersect(range2);

                // عرض معلومات حول التقاطع
                Console.WriteLine($"Intersection result range: {intersectionResult.RefersTo}");
                Console.WriteLine($"First row: {intersectionResult.FirstRow}");
                Console.WriteLine($"First column: {intersectionResult.FirstColumn}");
                Console.WriteLine($"Row count: {intersectionResult.RowCount}");
                Console.WriteLine($"Column count: {intersectionResult.ColumnCount}");

                // تمييز منطقة التقاطع
                Style highlightStyle = workbook.CreateStyle();
                highlightStyle.BackgroundColor = System.Drawing.Color.Yellow;
                intersectionResult.SetStyle(highlightStyle);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Intersect method: {ex.Message}");
            }

            // احفظ المصنف
            workbook.Save("UnionRangeMethodIntersectWithUnionRangeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Intersect(Range[]) {#intersect}

يتقاطع مع نطاق آخر.

```csharp
public UnionRange Intersect(Range[] ranges)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| نطاقات | Range[] | النطاق. |

### ملاحظات

إذا لم تتقاطع نطاقات الاتحاد الاثنين، تُعيد null.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodIntersectWithRangeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء بيانات عينة في الخلايا
            worksheet.Cells["A1"].PutValue("A1");
            worksheet.Cells["B1"].PutValue("B1");
            worksheet.Cells["A2"].PutValue("A2");
            worksheet.Cells["B2"].PutValue("B2");

            // إنشاء نطاقات للتقاطع
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B1");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("A1:A2");
            Aspose.Cells.Range[] rangesToIntersect = new Aspose.Cells.Range[] { range1, range2 };

            // الحصول على نطاق الاتحاد للورقة
            UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });

            try
            {
                // استدعاء طريقة Intersect مع معامل Range[]
                UnionRange intersectionResult = unionRange.Intersect(rangesToIntersect);

                // عرض معلومات حول نتيجة التقاطع
                Console.WriteLine($"Intersection result range: {intersectionResult.RefersTo}");
                Console.WriteLine($"First row: {intersectionResult.FirstRow}");
                Console.WriteLine($"First column: {intersectionResult.FirstColumn}");
                Console.WriteLine($"Row count: {intersectionResult.RowCount}");
                Console.WriteLine($"Column count: {intersectionResult.ColumnCount}");

                // تمييز منطقة التقاطع
                Style style = workbook.CreateStyle();
                style.BackgroundColor = System.Drawing.Color.Yellow;
                intersectionResult.SetStyle(style);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Intersect method: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("UnionRangeMethodIntersectWithRangeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Range](../../range/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


