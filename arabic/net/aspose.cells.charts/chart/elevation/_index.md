---
title: "Chart.Elevation"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Chart. تمثل ارتفاع عرض المخطط ثلاثي الأبعاد بالدرجات"
type: docs
url: /ar/net/aspose.cells.charts/chart/elevation/
---
## Chart.Elevation property

يمثل ارتفاع عرض المخطط ثلاثي الأبعاد، بالدرجات.

```csharp
public int Elevation { get; set; }
```

### ملاحظات

ارتفاع المخطط هو الارتفاع الذي تعرض المخطط منه، بالدرجات. القيمة الافتراضية هي 15 لمعظم أنواع المخططات. يجب أن تكون قيمة هذه الخاصية بين -90 و 90، باستثناء مخططات الأعمدة ثلاثية الأبعاد، حيث يجب أن تكون بين 0 و 44.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyElevationDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // إضافة مخطط عمودي ثلاثي الأبعاد
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // تعيين خاصية الارتفاع (الزاوية بالدرجات)
            chart.Elevation = 30;
            
            // احفظ المصنف
            workbook.Save("ChartElevationDemo.xlsx");

            Console.WriteLine("Chart created with elevation set to 30 degrees.");
        }
    }
}
```

### انظر أيضًا

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


