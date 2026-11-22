---
title: "الفئة Format3D"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Drawing.Format3D. تحدد هذه الفئة خصائص الشكل ثلاثي الأبعاد لعنصر مخطط أو شكل"
type: docs
url: /ar/net/aspose.cells.drawing/format3d/
---
## Format3D class

تحدد هذه الفئة خصائص الشكل ثلاثي الأبعاد لعنصر مخطط أو شكل.

```csharp
public class Format3D
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [LightingAngle](../../aspose.cells.drawing/format3d/lightingangle/) { get; set; } | يحصل ويضبط زاوية الإضاءة. النطاق من 0 إلى 359.9 درجة. |
| [SurfaceLightingType](../../aspose.cells.drawing/format3d/surfacelightingtype/) { get; set; } | يحصل ويضبط نوع الإضاءة الذي سيُطبق على مشهد الشكل. القيمة الافتراضية هي LightRigType.ThreePoint. |
| [SurfaceMaterialType](../../aspose.cells.drawing/format3d/surfacematerialtype/) { get; set; } | يحصل ويضبط نوع المادة الذي يُدمج مع خصائص الإضاءة لإعطاء المظهر والشعور النهائي للشكل. القيمة الافتراضية هي PresetMaterialType.WarmMatte. |
| [TopBevel](../../aspose.cells.drawing/format3d/topbevel/) { get; } | يحصل على كائن [`Bevel`](../bevel/) الذي يحتوي على الخصائص المرتبطة بتعريف الحافة على الوجه العلوي أو الأمامي للشكل. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [HasTopBevelData](../../aspose.cells.drawing/format3d/hastopbeveldata/)() | يشير إلى ما إذا كان الشكل يحتوي على بيانات الحافة العلوية. |

### أمثلة

```csharp
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System;

namespace AsposeCellsExamples
{
    public class Format3DDemo
    {
        public static void RunDemo()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بعض البيانات التجريبية
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);
            sheet.Cells["A4"].PutValue(40);

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = sheet.Charts.Add(ChartType.Column3DClustered, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];

            // إضافة سلسلة إلى المخطط
            chart.NSeries.Add("A1:A4", true);

            // الوصول إلى السلسلة الأولى
            Series series = chart.NSeries[0];

            // الوصول إلى تنسيق 3D للسلسلة
            Format3D format3D = series.ShapeProperties.Format3D;

            // تعيين خصائص تنسيق ثلاثي الأبعاد
            format3D.SurfaceMaterialType = PresetMaterialType.WarmMatte;
            format3D.SurfaceLightingType = LightRigType.ThreePoint;
            format3D.LightingAngle = 45.0;

            // تحقق مما إذا كان الشكل يحتوي على بيانات الحافة العلوية
            if (format3D.HasTopBevelData())
            {
                Bevel topBevel = format3D.TopBevel;
                Console.WriteLine("Top Bevel Width: " + topBevel.Width);
                Console.WriteLine("Top Bevel Height: " + topBevel.Height);
            }

            // احفظ المصنف
            workbook.Save("Format3DDemo.xlsx");
            workbook.Save("Format3DDemo.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


