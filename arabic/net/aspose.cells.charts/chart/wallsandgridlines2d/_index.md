---
title: "Chart.WallsAndGridlines2D"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Chart. True إذا تم رسم خطوط الشبكة ثنائي الأبعاد على مخطط ثلاثي الأبعاد"
type: docs
url: /ar/net/aspose.cells.charts/chart/wallsandgridlines2d/
---
## Chart.WallsAndGridlines2D property

صحيح إذا تم رسم خطوط الشبكة ثنائي الأبعاد على مخطط ثلاثي الأبعاد.

```csharp
public bool WallsAndGridlines2D { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyWallsAndGridlines2DDemo
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
            worksheet.Cells["B4"].PutValue(15);

            // أضف مخطط عمودي
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // عرض خاصية WallsAndGridlines2D
            chart.WallsAndGridlines2D = true; // Show walls and gridlines in 2D
            Console.WriteLine("WallsAndGridlines2D is set to: " + chart.WallsAndGridlines2D);

            // احفظ المصنف
            workbook.Save("WallsAndGridlines2DDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


