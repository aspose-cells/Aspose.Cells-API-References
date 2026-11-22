---
title: "Chart.RightAngleAxes"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Chart. صحيحة إذا كانت محاور المخطط بزاوية قائمة. ينطبق فقط على المخططات ثلاثية الأبعاد باستثناء Column3D ومخططات الفطيرة ثلاثية الأبعاد"
type: docs
url: /ar/net/aspose.cells.charts/chart/rightangleaxes/
---
## Chart.RightAngleAxes property

صحيح إذا كانت محاور المخطط عمودية على بعضها. ينطبق فقط على المخططات ثلاثية الأبعاد (باستثناء Column3D ومخططات الفطيرة ثلاثية الأبعاد).

```csharp
public bool RightAngleAxes { get; set; }
```

### ملاحظات

إذا كانت هذه الخاصية صحيحة، يتم تجاهل خاصية Perspective.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyRightAngleAxesDemo
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
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(35);

            // إضافة مخطط عمودي ثلاثي الأبعاد
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // عرض خاصية RightAngleAxes
            chart.RightAngleAxes = true;
            Console.WriteLine("RightAngleAxes is set to: " + chart.RightAngleAxes);

            // احفظ المصنف
            workbook.Save("RightAngleAxesDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


