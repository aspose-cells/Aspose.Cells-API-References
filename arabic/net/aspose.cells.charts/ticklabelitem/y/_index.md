---
title: "TickLabelItem.Y"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TickLabelItem. إحداثيات Y لعنصر Ticklabel كنسبة من ارتفاع المخطط"
type: docs
url: /ar/net/aspose.cells.charts/ticklabelitem/y/
---
## TickLabelItem.Y property

إحداثيات ص لعنصر Ticklabel كنسبة من ارتفاع المخطط.

```csharp
public double Y { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TickLabelItemPropertyYDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["A3"].PutValue("Category 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // أضف مخطط عمودي
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B1:B3", true);
            
            // تعيين بيانات محور الفئة باستخدام NSERIES بدلاً من CategoryData
            chart.NSeries.CategoryData = "A1:A3";

            // حساب المخطط لضمان إنشاء تسميات الفواصل
            chart.Calculate();

            // الحصول على عناصر تسميات الفواصل من محور الفئة
            Aspose.Cells.Charts.TickLabelItem[] tickLabelItems = chart.CategoryAxis.TickLabels.TickLabelItems;

            // إظهار استخدام خاصية Y بإضافة أشكال محاذاة مع تسميات الفواصل
            for (int i = 0; i < tickLabelItems.Length; i++)
            {
                Aspose.Cells.Charts.TickLabelItem item = tickLabelItems[i];
                
                // إضافة مستطيل عند كل موضع Y لتسمية الفاصل
                Shape shape = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.Rectangle, 
                    PlacementType.Move,
                    item.X,
                    item.Y, // Using the Y property of TickLabelItem
                    item.X + 0.05, // Small width
                    item.Y + 0.02); // Small height
                
                shape.Fill.SolidFill.Color = Color.FromArgb(100, 0, 255, 0); // Semi-transparent green
                shape.Line.SolidFill.Color = Color.Black;
            }

            // احفظ المصنف
            workbook.Save("TickLabelItemPropertyYDemo_Output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TickLabelItem](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


