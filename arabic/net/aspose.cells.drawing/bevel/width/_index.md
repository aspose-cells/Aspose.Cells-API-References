---
title: "Bevel.Width"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Bevel خاصية. يحصل ويضبط عرض الحافة أو مدى تطبيقها داخل الشكل. بوحدة النقاط"
type: docs
url: /ar/net/aspose.cells.drawing/bevel/width/
---
## Bevel.Width property

يحصل على عرض الحافة المائلة ويضبطه، أو مدى دخوله داخل الشكل عند تطبيقه. بوحدة النقاط.

```csharp
public double Width { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class BevelPropertyWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 5, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // احصل على السلسلة الأولى واضبط تنسيق ثلاثي الأبعاد
            Series series = chart.NSeries[0];
            Format3D format3D = series.ShapeProperties.Format3D;
            
            // تكوين خصائص الحافة باستخدام عرض توضيحي
            Bevel topBevel = format3D.TopBevel;
            topBevel.Type = BevelPresetType.Circle;
            topBevel.Width = 12; // Demonstrating Width property
            topBevel.Height = 6;

            // احفظ المصنف
            workbook.Save("BevelWidthDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Bevel](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


