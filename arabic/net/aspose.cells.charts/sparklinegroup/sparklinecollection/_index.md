---
title: "SparklineGroup.SparklineCollection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SparklineGroup. يحصل على مجموعة كائنات Sparkline"
type: docs
url: /ar/net/aspose.cells.charts/sparklinegroup/sparklinecollection/
---
## SparklineGroup.SparklineCollection property

يحصل على مجموعة كائن [`Sparkline`](../../sparkline/)

```csharp
[Obsolete("Use SparklineGroup.Sparklines property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public SparklineCollection SparklineCollection { get; }
```

### ملاحظات

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام خاصية SparklineGroup.Sparklines. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ نوفمبر 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SparklineGroupPropertySparklineCollectionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة للمخططات الصغيرة
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["B1"].PutValue(20);
            worksheet.Cells["C1"].PutValue(15);
            worksheet.Cells["D1"].PutValue(30);

            try
            {
                // تحديد موقع الـ sparklines
                CellArea location = new CellArea
                {
                    StartRow = 0,
                    EndRow = 0,
                    StartColumn = 4,
                    EndColumn = 4
                };

                // أضف مجموعة مخطط خطي إلى ورقة العمل.
                int groupIndex = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, location);
                SparklineGroup sparklineGroup = worksheet.SparklineGroups[groupIndex];

                // إضافة sparkline إلى المجموعة
                sparklineGroup.Sparklines.Add(worksheet.Name + "!A1:D1", 0, 4);

                // الوصول إلى خاصية SparklineCollection (للقراءة فقط)
                SparklineCollection sparklineCollection = sparklineGroup.SparklineCollection;

                // عرض معلومات حول مجموعة الـ sparkline
                Console.WriteLine($"SparklineCollection contains {sparklineCollection.Count} sparklines");

                // التكرار عبر الـ sparklines في المجموعة
                for (int i = 0; i < sparklineCollection.Count; i++)
                {
                    Sparkline sparkline = sparklineCollection[i];
                    Console.WriteLine($"Sparkline {i + 1} location: Row {sparkline.Row}, Column {sparkline.Column}");
                }

                // احفظ المصنف
                workbook.Save("SparklineCollectionDemo.xlsx");
                Console.WriteLine("SparklineCollection demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [SparklineCollection](../../sparklinecollection/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


