---
title: "ChartPoint.ArcEndPointYPx"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartPoint. تحصل على إحداثي y للنقطة النهائية لقسم الفطيرة بعد استدعاء طريقة Chart.Calculate. ينطبق على مخطط الفطيرة ومخطط الدونات."
type: docs
url: /ar/net/aspose.cells.charts/chartpoint/arcendpointypx/
---
## ChartPoint.ArcEndPointYPx property

يحصل على إحداثي y للنقطة النهائية لقسم الفطيرة بعد استدعاء طريقة Chart.Calculate(). ينطبق على مخطط الفطيرة والدونات.

```csharp
public float ArcEndPointYPx { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyArcEndPointYPxDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("C1");
            worksheet.Cells["A3"].PutValue("C2");
            worksheet.Cells["A4"].PutValue("C3");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(8000);
            worksheet.Cells["B3"].PutValue(12000);
            worksheet.Cells["B4"].PutValue(14000);

            // إضافة مخطط فطيرة
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // احسب المخطط للحصول على مواضع الأشكال.
            chart.Calculate();

            // احصل على أول نقطة في المخطط
            ChartPoint point = chart.NSeries[0].Points[0];

            // اعرض قيمة ArcEndPointYPx الحالية.
            Console.WriteLine("Current ArcEndPointYPx value: " + point.ArcEndPointYPx);

            // نظرًا لأن ArcEndPointYPx للقراءة فقط، لا يمكننا سوى قراءتها.
            // السطر التالي سيتسبب في خطأ تجميع:
            // point.ArcEndPointYPx = 150.5f;

            // أظهر كيف تؤثر هذه الخاصية على مخطط الفطيرة.
            Console.WriteLine("Pie slice end point Y coordinate: " + point.ArcEndPointYPx + " pixels");

            // احفظ المصنف
            workbook.Save("ChartPointPropertyArcEndPointYPxDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


