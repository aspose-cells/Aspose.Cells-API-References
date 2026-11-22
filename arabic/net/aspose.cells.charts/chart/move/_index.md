---
title: "Chart.Move"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة المخطط. تنقل المخطط إلى موقع محدد"
type: docs
url: /ar/net/aspose.cells.charts/chart/move/
---
## Chart.Move method

ينقل المخطط إلى موقع محدد.

```csharp
public void Move(int topRow, int leftColumn, int bottomRow, int rightColumn)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| العمود الأيسر | Int32 | فهرس العمود العلوي الأيسر. |
| topRow | Int32 | فهرس الصف العلوي الأيسر. |
| rightColumn | Int32 | فهرس العمود السفلي الأيمن |
| الصف السفلي | Int32 | فهرس الصف السفلي الأيمن |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartMethodMoveWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // الموضع الأصلي للمخطط
                Console.WriteLine($"Original position - topRow: {chart.ChartObject.UpperLeftRow}, leftColumn: {chart.ChartObject.UpperLeftColumn}");

                // نقل المخطط إلى موضع جديد (الصفوف 10-20، الأعمدة 2-8)
                chart.Move(10, 2, 20, 8);

                // عرض الموضع الجديد
                Console.WriteLine($"New position - topRow: {chart.ChartObject.UpperLeftRow}, leftColumn: {chart.ChartObject.UpperLeftColumn}");

                // احفظ المصنف
                workbook.Save("ChartMoveDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Move method: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


