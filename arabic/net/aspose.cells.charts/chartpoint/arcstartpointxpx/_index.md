---
title: "ChartPoint.ArcStartPointXPx"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartPoint. يحصل على إحداثي x للنقطة البداية لقسم الفطيرة بعد استدعاء طريقة Chart.Calculate. ينطبق على مخططات Pie و Doughnut."
type: docs
url: /ar/net/aspose.cells.charts/chartpoint/arcstartpointxpx/
---
## ChartPoint.ArcStartPointXPx property

يحصل على إحداثي x للنقطة الابتدائية لقسم الفطيرة بعد استدعاء طريقة Chart.Calculate(). ينطبق على مخططات الفطيرة والدونات.

```csharp
public float ArcStartPointXPx { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyArcStartPointXPxDemo
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
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // إضافة مخطط فطيرة
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // احسب المخطط لضمان تعبئة الخصائص
            chart.Calculate();

            // احصل على أول نقطة في المخطط
            ChartPoint point = chart.NSeries[0].Points[0];

            // اعرض قيمة ArcStartPointXPx
            Console.WriteLine("ArcStartPointXPx for first point: " + point.ArcStartPointXPx);

            // ملاحظة: ArcStartPointXPx للقراءة فقط، لذا لا يمكننا تعيينه مباشرةً
            // بدلاً من ذلك، يمكننا توضيح كيف يتغير عندما نقوم بتعديل خصائص أخرى

            // غيّر قيمة الانفجار التي تؤثر على موضع شريحة الفطيرة
            point.Explosion = 20;
            chart.Calculate(); // Recalculate to update properties

            // اعرض القيمة الجديدة لـ ArcStartPointXPx بعد تغيير الانفجار
            Console.WriteLine("ArcStartPointXPx after explosion: " + point.ArcStartPointXPx);

            // احفظ المصنف
            workbook.Save("ChartPointPropertyArcStartPointXPxDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


