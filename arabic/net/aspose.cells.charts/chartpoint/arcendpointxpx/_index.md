---
title: "ChartPoint.ArcEndPointXPx"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartPoint. يحصل على إحداثي x للنقطة النهائية لقسم الفطيرة بعد استدعاء طريقة Chart.Calculate. ينطبق على مخططات Pie و Doughnut"
type: docs
url: /ar/net/aspose.cells.charts/chartpoint/arcendpointxpx/
---
## ChartPoint.ArcEndPointXPx property

يحصل على إحداثي x للنقطة النهائية لقسم الفطيرة بعد استدعاء طريقة Chart.Calculate(). ينطبق على مخططات الفطيرة والدونات.

```csharp
public float ArcEndPointXPx { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyArcEndPointXPxDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // إضافة مخطط فطيرة
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // احسب المخطط لضمان تعبئة الخصائص
            chart.Calculate();

            // احصل على أول نقطة في المخطط
            ChartPoint point = chart.NSeries[0].Points[0];

            // اعرض قيمة ArcEndPointXPx
            Console.WriteLine("ArcEndPointXPx: " + point.ArcEndPointXPx);

            // ملاحظة: ArcEndPointXPx للقراءة فقط، لذا لا يمكننا تعيينه مباشرة
            // لتغيير نقطة النهاية، نحتاج إلى تعديل بيانات المخطط أو الخصائص التي تؤثر على شريحة الفطيرة
            
            // مثال على كيفية تأثير تغيير البيانات على ArcEndPointXPx
            worksheet.Cells["B2"].PutValue(60); // Increase Apple's value
            chart.Calculate(); // Recalculate chart

            // اعرض القيمة الجديدة لـ ArcEndPointXPx بعد تغيير البيانات
            Console.WriteLine("New ArcEndPointXPx after data change: " + point.ArcEndPointXPx);

            // احفظ المصنف
            workbook.Save("ChartPointPropertyArcEndPointXPxDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


