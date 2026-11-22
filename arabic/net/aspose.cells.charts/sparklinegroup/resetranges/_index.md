---
title: "SparklineGroup.ResetRanges"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SparklineGroup. تعيد ضبط نطاق البيانات ونطاق الموقع لمجموعة الـ sparkline. ستقوم هذه الطريقة بمسح عناصر الـ sparkline الأصلية في المجموعة وإنشاء عناصر sparkline جديدة للنطاقات الجديدة"
type: docs
url: /ar/net/aspose.cells.charts/sparklinegroup/resetranges/
---
## SparklineGroup.ResetRanges method

يعيد تعيين نطاق البيانات ونطاق الموقع لمجموعة المخططات الخطية. ستقوم هذه الطريقة بمسح عناصر المخطط الخطي الأصلية في المجموعة وإنشاء عناصر مخطط خطي جديدة للنطاقات الجديدة.

```csharp
public void ResetRanges(string dataRange, bool isVertical, CellArea locationRange)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| dataRange | String | يحدد نطاق البيانات الجديد لمجموعة الـ sparkline. |
| isVertical | منطقي | يحدد ما إذا كان سيتم رسم الـ sparklines من نطاق البيانات الجديد حسب الصف أو حسب العمود. |
| locationRange | CellArea | يحدد مكان وضع المخططات الصغيرة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SparklineGroupMethodResetRangesWithStringBooleanCellAreaDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة بعض البيانات إلى ورقة العمل
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // حدد CellArea للمخطط الخطي.
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // أضف مجموعة مخطط خطي إلى ورقة العمل.
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);

            SparklineGroup group = sheet.SparklineGroups[idx];

            // تحضير المعلمات لـ ResetRanges
            string dataRange = "A1:D1";
            bool isVertical = false;
            CellArea locationRange = CellArea.CreateCellArea(6, 5, 6, 5);

            try
            {
                // استدعاء ResetRanges مع المعلمات (String, Boolean, CellArea)
                group.ResetRanges(dataRange, isVertical, locationRange);

                Console.WriteLine("ResetRanges method executed successfully with parameters (String, Boolean, CellArea)");
                
                
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ResetRanges method: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("SparklineGroupResetRangesDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


