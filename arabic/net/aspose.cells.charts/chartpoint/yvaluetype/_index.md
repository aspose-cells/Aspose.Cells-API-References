---
title: "ChartPoint.YValueType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartPoint. تحصل على نوع قيمة Y لنقطة المخطط"
type: docs
url: /ar/net/aspose.cells.charts/chartpoint/yvaluetype/
---
## ChartPoint.YValueType property

يحصل على نوع قيمة Y لنقطة المخطط.

```csharp
public CellValueType YValueType { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyYValueTypeDemo
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

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // احصل على أول نقطة في المخطط في السلسلة الأولى
            ChartPoint chartPoint = chart.NSeries[0].Points[0];

            // اعرض نوع YValueType الحالي
            Console.WriteLine("Current YValueType: " + chartPoint.YValueType);

            // اعرض YValue قبل التغيير
            Console.WriteLine("Current YValue: " + chartPoint.YValue);

            // غيّر YValue إلى نوع مختلف (string لتوضيح تغيير النوع)
            chartPoint.YValue = "15"; // This will change the YValueType to IsString

            // اعرض YValueType بعد التغيير
            Console.WriteLine("New YValueType: " + chartPoint.YValueType);
            Console.WriteLine("New YValue: " + chartPoint.YValue);

            // احفظ المصنف
            workbook.Save("ChartPointPropertyYValueTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [CellValueType](../../../aspose.cells/cellvaluetype/)
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


