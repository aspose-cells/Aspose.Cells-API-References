---
title: "التعداد LightRigType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.Drawing.LightRigType. يمثل إعداد إضاءة مسبق يمكن تطبيقه على شكل"
type: docs
url: /ar/net/aspose.cells.drawing/lightrigtype/
---
## LightRigType enumeration

يمثل إضاءة مسبقة إلى اليمين يمكن تطبيقها على الشكل.

```csharp
public enum LightRigType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Balanced | `0` | متوازن |
| BrightRoom | `1` | غرفة مشرقة |
| Chilly | `2` | بارد |
| Contrasting | `3` | متباين |
| Flat | `4` | مسطح |
| Flood | `5` | فيضان |
| Freezing | `6` | متجمد |
| Glow | `7` | توهج |
| Harsh | `8` | قاسي |
| LegacyFlat1 | `9` | LegacyFlat1 |
| LegacyFlat2 | `10` | LegacyFlat2 |
| LegacyFlat3 | `11` | LegacyFlat3 |
| LegacyFlat4 | `12` | LegacyFlat4 |
| LegacyHarsh1 | `13` | LegacyHarsh1 |
| LegacyHarsh2 | `14` | LegacyHarsh2 |
| LegacyHarsh3 | `15` | LegacyHarsh3 |
| LegacyHarsh4 | `16` | LegacyHarsh4 |
| LegacyNormal1 | `17` | LegacyNormal1 |
| LegacyNormal2 | `18` | LegacyNormal2 |
| LegacyNormal3 | `19` | LegacyNormal3 |
| LegacyNormal4 | `20` | LegacyNormal4 |
| Morning | `21` | صباح |
| Soft | `22` | ناعم |
| Sunrise | `23` | شروق الشمس |
| Sunset | `24` | غروب الشمس |
| ThreePoint | `25` | ثلاث نقاط |
| TwoPoint | `26` | نقطتين |
| None | `27` | لا توجد مجموعة إضاءة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class LightRigTypeDemo
    {
        public static void LightRigTypeExample()
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين نطاق بيانات المخطط
            chart.SetChartDataRange("A1:B4", true);

            // الوصول إلى السلسلة الأولى في المخطط
            Series series = chart.NSeries[0];

            // الوصول إلى خصائص الشكل للسلسلة
            ShapePropertyCollection shapeProperties = series.ShapeProperties;

            // تحقق مما إذا كانت السلسلة تحتوي على بيانات تنسيق ثلاثي الأبعاد
            if (shapeProperties.HasFormat3D())
            {
                // الوصول إلى خصائص تنسيق ثلاثي الأبعاد
                Format3D format3D = shapeProperties.Format3D;

                // ضبط نوع إضاءة السطح إلى متوازن
                format3D.SurfaceLightingType = LightRigType.Balanced;

                // ضبط زاوية الإضاءة
                format3D.LightingAngle = 45.0;
            }

            // احفظ المصنف
            workbook.Save("LightRigTypeExample.xlsx");
            workbook.Save("LightRigTypeExample.pdf");
            // أخرج النتائج
            Console.WriteLine("LightRigType example applied and workbook saved as 'LightRigTypeExample.xlsx'.");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


