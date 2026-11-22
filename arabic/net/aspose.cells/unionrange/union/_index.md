---
title: "UnionRange.Union"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة UnionRange. دمج نطاق آخر"
type: docs
url: /ar/net/aspose.cells/unionrange/union/
---
## Union(string) {#union_2}

اتحاد نطاق آخر.

```csharp
public UnionRange Union(string range)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| نطاق | String | النطاق. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodUnionWithStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء نطاق أولي وتعبئته بالبيانات
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B2");
            range1[0, 0].PutValue("Range1");
            range1[0, 1].PutValue(100);
            range1[1, 0].PutValue("Data");
            range1[1, 1].PutValue(200);

            // إنشاء UnionRange من النطاق الأولي
            UnionRange unionRange = worksheet.Cells.CreateRange(range1.RefersTo).UnionRanges(new Aspose.Cells.Range[] { range1 });

            try
            {
                // استدعاء طريقة Union مع معلمة نصية تمثل نطاقًا آخر
                UnionRange combinedRange = unionRange.Union("C1:D2");

                // تعبئة النطاق الثاني بالبيانات
                worksheet.Cells["C1"].PutValue("Range2");
                worksheet.Cells["D1"].PutValue(300);
                worksheet.Cells["C2"].PutValue("More");
                worksheet.Cells["D2"].PutValue(400);

                Console.WriteLine("Union method executed successfully with parameter (String)");
                Console.WriteLine($"Combined range refers to: {combinedRange.RefersTo}");
                Console.WriteLine($"Total ranges in union: {combinedRange.RangeCount}");

                // عرض المعلومات حول النطاق المدمج
                Console.WriteLine("\nCombined Range Info:");
                Console.WriteLine($"FirstRow: {combinedRange.FirstRow}, FirstColumn: {combinedRange.FirstColumn}");
                Console.WriteLine($"RowCount: {combinedRange.RowCount}, ColumnCount: {combinedRange.ColumnCount}");
                Console.WriteLine($"CellCount: {combinedRange.CellCount}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Union method: {ex.Message}");
            }

            // احفظ المصنف
            workbook.Save("UnionRangeMethodUnionWithStringDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Union(UnionRange) {#union_1}

اتحاد نطاق آخر.

```csharp
public UnionRange Union(UnionRange unionRange)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| unionRange | UnionRange | النطاق. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodUnionWithUnionRangeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء النطاق الأول وتعبئته بالبيانات
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B2");
            range1[0, 0].PutValue("Range1");
            range1[0, 1].PutValue(100);
            range1[1, 0].PutValue("Data");
            range1[1, 1].PutValue(200);

            // إنشاء النطاق الثاني وتعبئته بالبيانات
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("C1:D2");
            range2[0, 0].PutValue("Range2");
            range2[0, 1].PutValue(300);
            range2[1, 0].PutValue("More");
            range2[1, 1].PutValue(400);

            // إنشاء UnionRange من النطاق الأول
            UnionRange unionRange1 = worksheet.Cells.CreateRange(range1.RefersTo).UnionRanges(new Aspose.Cells.Range[] { range1 });

            // إنشاء UnionRange من النطاق الثاني
            UnionRange unionRange2 = worksheet.Cells.CreateRange(range2.RefersTo).UnionRanges(new Aspose.Cells.Range[] { range2 });

            try
            {
                // استدعاء طريقة Union مع معلمة UnionRange
                UnionRange combinedRange = unionRange1.Union(unionRange2);

                Console.WriteLine("Union method executed successfully with parameter (UnionRange)");
                Console.WriteLine($"Combined range refers to: {combinedRange.RefersTo}");
                Console.WriteLine($"Total ranges in union: {combinedRange.RangeCount}");

                // عرض المعلومات حول النطاق المدمج
                Console.WriteLine("\nCombined Range Info:");
                Console.WriteLine($"FirstRow: {combinedRange.FirstRow}, FirstColumn: {combinedRange.FirstColumn}");
                Console.WriteLine($"RowCount: {combinedRange.RowCount}, ColumnCount: {combinedRange.ColumnCount}");
                Console.WriteLine($"CellCount: {combinedRange.CellCount}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Union method: {ex.Message}");
            }

            // احفظ المصنف
            workbook.Save("UnionRangeMethodUnionWithUnionRangeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Union(Range[]) {#union}

اتحاد النطاقات.

```csharp
public UnionRange Union(Range[] ranges)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| نطاقات | Range[] | النطاقات. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodUnionWithRangeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء نطاقات نموذجية لتوضيح الدمج
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B2");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("C3:D4");
            Aspose.Cells.Range range3 = worksheet.Cells.CreateRange("E5:F6");

            // وضع القيم في النطاقات لتصوّرها
            range1[0, 0].PutValue("Range1");
            range2[0, 0].PutValue("Range2");
            range3[0, 0].PutValue("Range3");

            try
            {
                // إنشاء نطاق دمج أولي
                UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { range1 });

                // استدعاء طريقة Union مع معلمة Range[]
                Aspose.Cells.Range[] rangesToUnion = new Aspose.Cells.Range[] { range2, range3 };
                UnionRange resultUnion = unionRange.Union(rangesToUnion);

                Console.WriteLine("Union method executed successfully with parameters (Range[])");
                Console.WriteLine($"Resulting union range count: {resultUnion.RangeCount}");
                Console.WriteLine($"Resulting union refers to: {resultUnion.RefersTo}");

                // قم بتمييز نتيجة الاتحاد عن طريق تعيين لون الخلفية
                Style highlightStyle = workbook.CreateStyle();
                highlightStyle.ForegroundColor = System.Drawing.Color.LightYellow;
                highlightStyle.Pattern = BackgroundType.Solid;
                resultUnion.SetStyle(highlightStyle);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Union method: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("UnionRangeMethodUnionWithRangeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Range](../../range/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


