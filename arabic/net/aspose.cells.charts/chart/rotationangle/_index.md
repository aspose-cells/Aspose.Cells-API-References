---
title: "Chart.RotationAngle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Chart. تمثل دوران عرض المخطط ثلاثي الأبعاد، دوران مساحة الرسم حول المحور Z بالدرجات"
type: docs
url: /ar/net/aspose.cells.charts/chart/rotationangle/
---
## Chart.RotationAngle property

يمثل دوران عرض المخطط ثلاثي الأبعاد (دوران منطقة المخطط حول المحور z، بالدرجات).

```csharp
public int RotationAngle { get; set; }
```

### ملاحظات

يجب أن تكون قيمة هذه الخاصية من 0 إلى 360، باستثناء مخططات الأشرطة ثلاثية الأبعاد، حيث يجب أن تكون القيمة من 0 إلى 44. القيمة الافتراضية هي 20. ينطبق فقط على المخططات ثلاثية الأبعاد.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyRotationAngleDemo
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

            // إضافة مخطط عمودي ثلاثي الأبعاد
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // تعيين زاوية الدوران إلى 45 درجة
            chart.RotationAngle = 45;

            // احفظ المصنف
            workbook.Save("ChartRotationAngleDemo.xlsx");

            Console.WriteLine("Chart with rotation angle created successfully.");
        }
    }
}
```

### انظر أيضًا

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


