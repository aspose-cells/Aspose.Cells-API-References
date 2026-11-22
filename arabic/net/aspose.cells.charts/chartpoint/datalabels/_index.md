---
title: "ChartPoint.DataLabels"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartPoint. تُرجع كائن DataLabels الذي يمثل تسمية البيانات المرتبطة بهذه النقطة المخططة"
type: docs
url: /ar/net/aspose.cells.charts/chartpoint/datalabels/
---
## ChartPoint.DataLabels property

تُرجع كائن `DataLabels` الذي يمثل تسمية البيانات المرتبطة بهذه النقطة المخططة.

```csharp
public DataLabels DataLabels { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyDataLabelsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // أضف مخطط عمودي
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // الوصول إلى أول نقطة مخطط
                ChartPoint point = chart.NSeries[0].Points[0];

                // احصل على خاصية DataLabels (للقراءة فقط)
                DataLabels dataLabels = point.DataLabels;

                // عرض خصائص DataLabels
                Console.WriteLine("DataLabels ShowValue: " + dataLabels.ShowValue);
                Console.WriteLine("DataLabels ShowCategoryName: " + dataLabels.ShowCategoryName);
                Console.WriteLine("DataLabels ShowSeriesName: " + dataLabels.ShowSeriesName);
                Console.WriteLine("DataLabels Position: " + dataLabels.Position);

                // عدّل بعض خصائص DataLabels (نظرًا لأن DataLabels ليست للقراءة فقط)
                dataLabels.ShowValue = true;
                dataLabels.ShowCategoryName = true;
                dataLabels.Position = LabelPositionType.OutsideEnd;

                // حفظ النتيجة
                workbook.Save("ChartPointDataLabelsDemo.xlsx");
                Console.WriteLine("DataLabels demonstration completed successfully.");
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

* class [DataLabels](../../datalabels/)
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


