---
title: "التعداد BevelPresetType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.Drawing.BevelPresetType. تمثّل إعدادًا مسبقًا لنوع الحافة التي يمكن تطبيقها على شكل في 3D"
type: docs
url: /ar/net/aspose.cells.drawing/bevelpresettype/
---
## BevelPresetType enumeration

يمثل إعدادًا مسبقًا لنوع الحافة التي يمكن تطبيقها على شكل ثلاثي الأبعاد.

```csharp
public enum BevelPresetType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| None | `0` | بدون حافة |
| Angle | `1` | زاوية |
| ArtDeco | `2` | آرت ديكو |
| Circle | `3` | دائرة |
| Convex | `4` | محدب |
| CoolSlant | `5` | انحدار أنيق |
| Cross | `6` | صليب |
| Divot | `7` | ثقب |
| HardEdge | `8` | حافة صلبة |
| RelaxedInset | `9` | إدراج مريح |
| Riblet | `10` | خط رفيع |
| Slope | `11` | منحدر |
| SoftRound | `12` | دائري ناعم |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Charts;
    using System;

    public class BevelPresetTypeDemo
    {
        public static void BevelPresetTypeExample()
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

            // الوصول إلى عنوان المخطط وتعيين نصه
            chart.Title.Text = "Sample Chart with Bevel";

            // الوصول إلى منطقة رسم المخطط
            PlotArea plotArea = chart.PlotArea;

            // الوصول إلى خصائص الشكل لمنطقة المخطط
            ShapePropertyCollection shapeProperties = plotArea.ShapeProperties;

            
            // الوصول إلى خصائص تنسيق ثلاثي الأبعاد
            Format3D format3D = shapeProperties.Format3D;

            // الوصول إلى خصائص الحافة العلوية
            Bevel topBevel = format3D.TopBevel;

            // تعيين نوع الحافة إلى \"Angle\"
            topBevel.Type = BevelPresetType.Angle;

            // تعيين عرض وارتفاع الحافة
            topBevel.Width = 10;
            topBevel.Height = 10;

            // احفظ المصنف
            workbook.Save("BevelPresetTypeExample.xlsx");
            workbook.Save("BevelPresetTypeExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


