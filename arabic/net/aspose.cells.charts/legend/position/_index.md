---
title: "Legend.Position"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Legend. تحصل أو تضبط نوع موضع الأسطورة"
type: docs
url: /ar/net/aspose.cells.charts/legend/position/
---
## Legend.Position property

يحصل أو يضبط نوع موضع وسيلة الإيضاح.

```csharp
public LegendPositionType Position { get; set; }
```

### ملاحظات

الموضع الافتراضي هو اليمين. إذا كانت الأسطورة على الجانب الأيسر أو الأيمن من المخطط، فإن ضبط الخاصية Legend.X لن يكون له تأثير. إذا كانت الأسطورة على الجانب العلوي أو السفلي من المخطط، فإن ضبط الخاصية Legend.Y لن يكون له تأثير.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LegendPropertyPositionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // إضافة مخطط
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // ضبط موضع الأسطورة
            chart.Legend.Position = LegendPositionType.Left;

            // احفظ المصنف
            workbook.Save("LegendPositionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [LegendPositionType](../../legendpositiontype/)
* class [Legend](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


