---
title: "Chart.SideWall"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية المخطط. تُرجع كائن Walls الذي يمثل الجدار الجانبي لمخطط ثلاثي الأبعاد"
type: docs
url: /ar/net/aspose.cells.charts/chart/sidewall/
---
## Chart.SideWall property

تُرجع كائن [`Walls`](../walls/) الذي يمثل الجدار الجانبي لمخطط ثلاثي الأبعاد.

```csharp
public Walls SideWall { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPropertySideWallDemo
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
            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);
            worksheet.Cells["C1"].PutValue("Series 2");
            worksheet.Cells["C2"].PutValue(150);
            worksheet.Cells["C3"].PutValue(250);
            worksheet.Cells["C4"].PutValue(350);

            // إضافة مخطط عمودي ثلاثي الأبعاد
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.SetChartDataRange("A1:C4", true);

            // الوصول إلى خاصية SideWall
            Walls sideWall = chart.SideWall;
            
            // عرض بعض خصائص SideWall
            Console.WriteLine("SideWall properties:");
            Console.WriteLine("Width: " + sideWall.Width);
            Console.WriteLine("Height: " + sideWall.Height);
            Console.WriteLine("Depth: " + sideWall.Depth);

            // احسب المخطط لتحديث أبعاد الجدار
            chart.Calculate();

            // اعرض الخصائص المحدثة بعد الحساب
            Console.WriteLine("\nAfter Calculate():");
            Console.WriteLine("SideWall CenterX: " + sideWall.CenterX);
            Console.WriteLine("SideWall CenterY: " + sideWall.CenterY);
            Console.WriteLine("SideWall WidthPx: " + sideWall.WidthPx);
            Console.WriteLine("SideWall HeightPx: " + sideWall.HeightPx);

            // احفظ المصنف
            workbook.Save("ChartPropertySideWallDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Walls](../../walls/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


