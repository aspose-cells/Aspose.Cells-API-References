---
title: "تعداد ChartSplitType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Charts.ChartSplitType تعداد. يمثل الطريقة التي يتم بها تقسيم القسمين في مخطط فطيرة داخل فطيرة أو مخطط شريط داخل فطيرة"
type: docs
url: /ar/net/aspose.cells.charts/chartsplittype/
---
## ChartSplitType enumeration

يمثل الطريقة التي يتم بها تقسيم القسمين إما في مخطط فطيرة داخل فطيرة أو مخطط شريط داخل فطيرة.

```csharp
public enum ChartSplitType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Position | `0` | يمثل نقاط البيانات. يجب تقسيم نقاط البيانات بين الفطيرة والمخطط الثاني بوضع آخر موضع تقسيم لنقاط البيانات في المخطط الثاني. |
| Value | `1` | يمثل نقاط البيانات التي يجب تقسيمها بين الفطيرة والمخطط الثاني بوضع نقاط البيانات ذات القيمة الأقل من موضع التقسيم في المخطط الثاني. |
| PercentValue | `2` | يمثل نقاط البيانات التي يجب تقسيمها بين الفطيرة والمخطط الثاني بوضع النقاط التي نسبتها أقل من النسبة المئوية لموضع التقسيم في المخطط الثاني. |
| Custom | `3` | يمثل نقاط البيانات التي يجب تقسيمها بين الفطيرة والمخطط الثاني وفقاً لقيم التقسيم المخصصة. |
| Auto | `4` | يمثل نقاط البيانات التي يجب تقسيمها باستخدام الآلية الافتراضية لهذا النوع من المخططات. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartsClassChartSplitTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // إضافة بيانات نموذجية للمخطط
                worksheet.Cells["A1"].PutValue("Category");
                worksheet.Cells["A2"].PutValue("A");
                worksheet.Cells["A3"].PutValue("B");
                worksheet.Cells["A4"].PutValue("C");
                worksheet.Cells["A5"].PutValue("D");

                worksheet.Cells["B1"].PutValue("Value");
                worksheet.Cells["B2"].PutValue(10);
                worksheet.Cells["B3"].PutValue(20);
                worksheet.Cells["B4"].PutValue(30);
                worksheet.Cells["B5"].PutValue(40);

                // إضافة مخطط فطيرة
                int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
                Chart chart = worksheet.Charts[chartIndex];

                // تعيين نطاق بيانات المخطط
                chart.NSeries.Add("B2:B5", true);
                chart.NSeries.CategoryData = "A2:A5";

                // عرض قيم ChartSplitType المختلفة
                chart.NSeries[0].SplitType = ChartSplitType.Position;
                Console.WriteLine($"Current SplitType: {chart.NSeries[0].SplitType}");

                // تغيير إلى نوع تقسيم آخر
                chart.NSeries[0].SplitType = ChartSplitType.PercentValue;
                Console.WriteLine($"Updated SplitType: {chart.NSeries[0].SplitType}");

                // احفظ المصنف
                workbook.Save("ChartSplitTypeDemo.xlsx");
                Console.WriteLine("ChartSplitType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in ChartSplitType demonstration: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


