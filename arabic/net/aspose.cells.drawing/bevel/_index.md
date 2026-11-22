---
title: "الفئة Bevel"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Drawing.Bevel. تمثل حافة مائلة لشكل"
type: docs
url: /ar/net/aspose.cells.drawing/bevel/
---
## Bevel class

يمثل حافة مائلة للشكل

```csharp
public class Bevel
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Height](../../aspose.cells.drawing/bevel/height/) { get; set; } | يحصل على ارتفاع الحافة المائلة ويضبطه، أو مدى ارتفاعه فوق الشكل عند تطبيقه. بوحدة النقاط. |
| [Type](../../aspose.cells.drawing/bevel/type/) { get; set; } | يحصل على نوع الحافة المائلة المحدد مسبقًا ويضبطه. |
| [Width](../../aspose.cells.drawing/bevel/width/) { get; set; } | يحصل على عرض الحافة المائلة ويضبطه، أو مدى دخوله داخل الشكل عند تطبيقه. بوحدة النقاط. |

### أمثلة

```csharp
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System;

namespace AsposeCellsExamples
{
    public class BevelDemo
    {
        public static void RunDemo()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات التجريبية
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            workbook.CalculateFormula();

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // إضافة سلسلة بيانات إلى المخطط.
            chart.NSeries.Add("A1:B4", true);

            // الوصول إلى منطقة رسم المخطط
            ChartFrame plotArea = chart.PlotArea;

            // الوصول إلى خصائص الشكل لمنطقة المخطط
            ShapePropertyCollection shapeProperties = plotArea.ShapeProperties;

            // الوصول إلى خصائص تنسيق ثلاثي الأبعاد
            Format3D format3D = shapeProperties.Format3D;

            // الوصول إلى خصائص الحافة العلوية
            Bevel topBevel = format3D.TopBevel;

            // حدد العرض والارتفاع ونوع الحافة المائلة
            topBevel.Width = 10.0;
            topBevel.Height = 5.0;
            topBevel.Type = BevelPresetType.Circle;

            // حدد خصائص تنسيق ثلاثي الأبعاد الأخرى
            format3D.SurfaceMaterialType = PresetMaterialType.WarmMatte;
            format3D.SurfaceLightingType = LightRigType.ThreePoint;
            format3D.LightingAngle = 45.0;

            // احفظ المصنف
            workbook.Save("BevelDemo.xlsx");
            workbook.Save("BevelDemo.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


