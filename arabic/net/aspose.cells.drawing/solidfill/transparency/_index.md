---
title: "SolidFill.Transparency"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SolidFill. تُرجع أو تضبط درجة شفافية المنطقة كقيمة من 0.0 غير شفاف إلى 1.0 شفاف"
type: docs
url: /ar/net/aspose.cells.drawing/solidfill/transparency/
---
## SolidFill.Transparency property

يعيد أو يضبط درجة شفافية المنطقة كقيمة من 0.0 (معتم) إلى 1.0 (شفاف).

```csharp
public double Transparency { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SolidFillPropertyTransparencyDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف مخططًا تجريبيًا
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            chart.Calculate();

            // أضف شكلاً لإظهار الشفافية
            Shape shape = chart.Shapes.AddShapeInChart(MsoDrawingType.Rectangle, PlacementType.FreeFloating, 
                1000, 1000, 2000, 2000);
            
            // تعيين ملء صلب مع الشفافية
            shape.Fill.SolidFill.Color = Color.Blue;
            shape.Fill.SolidFill.Transparency = 0.5; // 50% transparent

            // إضافة شكل آخر للمقارنة (غير شفاف بالكامل)
            Shape shape2 = chart.Shapes.AddShapeInChart(MsoDrawingType.Rectangle, PlacementType.FreeFloating, 
                3000, 1000, 2000, 2000);
            shape2.Fill.SolidFill.Color = Color.Blue;
            shape2.Fill.SolidFill.Transparency = 0; // 0% transparent (fully opaque)

            // احفظ المصنف
            workbook.Save("SolidFillTransparencyDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SolidFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


