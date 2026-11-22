---
title: "ChartPoint.XValueType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartPoint. تحصل على نوع قيمة X لنقطة المخطط"
type: docs
url: /ar/net/aspose.cells.charts/chartpoint/xvaluetype/
---
## ChartPoint.XValueType property

يحصل على نوع قيمة X لنقطة المخطط.

```csharp
public CellValueType XValueType { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyXValueTypeDemo
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

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // احصل على أول نقطة في المخطط
            ChartPoint point = chart.NSeries[0].Points[0];

            // عرض قيمة XValueType الحالية
            Console.WriteLine("Current XValueType: " + point.XValueType);

            // تعيين XValue جديد (سيؤدي ذلك تلقائيًا إلى تحديث XValueType)
            point.XValue = DateTime.Now; // Changing to DateTime type
            Console.WriteLine("After setting DateTime value, XValueType: " + point.XValueType);

            point.XValue = "New Category"; // Changing to String type
            Console.WriteLine("After setting String value, XValueType: " + point.XValueType);

            point.XValue = 123.45; // Changing to Numeric type
            Console.WriteLine("After setting Numeric value, XValueType: " + point.XValueType);

            // احفظ المصنف
            workbook.Save("ChartPointXValueTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [CellValueType](../../../aspose.cells/cellvaluetype/)
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


