---
title: "Bevel.Height"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Bevel خاصية. يحصل ويضبط ارتفاع الحافة أو مدى تطبيقها فوق الشكل. بوحدة النقاط"
type: docs
url: /ar/net/aspose.cells.drawing/bevel/height/
---
## Bevel.Height property

يحصل على ارتفاع الحافة المائلة ويضبطه، أو مدى ارتفاعه فوق الشكل عند تطبيقه. بوحدة النقاط.

```csharp
public double Height { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class BevelPropertyHeightDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(1500);

            // إضافة مخطط عمودي ثلاثي الأبعاد
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // الوصول إلى تنسيق ثلاثي الأبعاد لمنطقة المخطط
            Format3D format3D = chart.PlotArea.ShapeProperties.Format3D;

            // تكوين الحافة العلوية باستخدام خاصية الارتفاع
            Bevel topBevel = format3D.TopBevel;
            topBevel.Type = BevelPresetType.ArtDeco;
            topBevel.Width = 8;
            topBevel.Height = 4.5; // Demonstrating Height property usage

            // احفظ المصنف
            workbook.Save("BevelHeightDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Bevel](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


