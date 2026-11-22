---
title: "Enum PresetMaterialType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Drawing.PresetMaterialType. يصف مظهر سطح الشكل"
type: docs
url: /ar/net/aspose.cells.drawing/presetmaterialtype/
---
## PresetMaterialType enumeration

يصف مظهر سطح الشكل.

```csharp
public enum PresetMaterialType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Clear | `0` | مسح |
| DarkEdge | `1` | حافة داكنة |
| Flat | `2` | مسطح |
| LegacyMatte | `3` | مات تقليدي |
| LegacyMetal | `4` | معدن تقليدي |
| LegacyPlastic | `5` | بلاستيك تقليدي |
| LegacyWireframe | `6` | إطار سلكي تقليدي |
| Matte | `7` | مات |
| Metal | `8` | معدن |
| Plastic | `9` | بلاستيك |
| Powder | `10` | بودرة |
| SoftEdge | `11` | حافة ناعمة |
| SoftMetal | `12` | معدن ناعم |
| TranslucentPowder | `13` | بودرة شبه شفافة |
| WarmMatte | `14` | مات دافئ |

### أمثلة

```csharp
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System;

namespace AsposeCellsExamples
{
    public class PresetMaterialTypeDemo
    {
        public static void PresetMaterialTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إضافة ورقة عمل جديدة إلى المصنف
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين نطاق بيانات المخطط
            chart.SetChartDataRange("A1:B4", true);

            // الوصول إلى السلسلة الأولى في المخطط
            Series series = chart.NSeries[0];

            // الوصول إلى تنسيق 3D للسلسلة
            Format3D format3D = series.ShapeProperties.Format3D;

            // تعيين نوع مادة السطح
            format3D.SurfaceMaterialType = PresetMaterialType.Metal;

            // تعيين خصائص 3D الأخرى
            format3D.LightingAngle = 45;
            format3D.SurfaceLightingType = LightRigType.ThreePoint;

            // احفظ المصنف
            workbook.Save("PresetMaterialTypeExample.xlsx");

            // أخرج النتائج
            Console.WriteLine("Chart with 3D format and PresetMaterialType applied has been created.");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


