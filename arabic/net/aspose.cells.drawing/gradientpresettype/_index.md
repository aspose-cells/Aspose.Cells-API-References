---
title: "تعداد GradientPresetType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Drawing.GradientPresetType. يمثل نوع لون التدرج المسبق"
type: docs
url: /ar/net/aspose.cells.drawing/gradientpresettype/
---
## GradientPresetType enumeration

يمثل نوع لون مسبق للتدرج.

```csharp
public enum GradientPresetType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Brass | `0` | لون مسبق للنحاس الأصفر |
| CalmWater | `1` | لون مسبق للمياه الهادئة |
| Chrome | `2` | لون مسبق للكروم |
| ChromeII | `3` | لون مسبق للكروم II |
| Daybreak | `4` | لون مسبق لفجر الصباح |
| Desert | `5` | لون مسبق للصحراء |
| EarlySunset | `6` | لون مسبق لغروب الشمس المبكر |
| Fire | `7` | لون مسبق للنار |
| Fog | `8` | لون مسبق للضباب |
| Gold | `9` | لون مسبق للذهب |
| GoldII | `10` | لون مسبق للذهب II |
| Horizon | `11` | لون مسبق للأفق |
| LateSunset | `12` | لون مسبق لغروب الشمس المتأخر |
| Mahogany | `13` | لون مسبق للماهوجني |
| Moss | `14` | لون مسبق للطحلب |
| Nightfall | `15` | لون مسبق للغسق |
| Ocean | `16` | لون مسبق للمحيط |
| Parchment | `17` | لون مسبق للرق |
| Peacock | `18` | لون مسبق للطاووس |
| Rainbow | `19` | لون مسبق لقوس قزح |
| RainbowII | `20` | لون مسبق لقوس قزح II |
| Sapphire | `21` | لون مسبق للياقوت |
| Silver | `22` | لون مسبق للفضة |
| Wheat | `23` | لون مسبق للقمح |
| Unknown | `24` | لون مسبق غير معروف. يُستخدم فقط للون المسبق (الذي لا يطابق أي لون مسبق معروف) في دفتر العمل القالب. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientPresetTypeDemo
    {
        public static void GradientPresetTypeExample()
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

            // الوصول إلى محور الفئات في المخطط
            Axis categoryAxis = chart.CategoryAxis;

            // الوصول إلى تنسيق التعبئة لمنطقة محور الفئات
            FillFormat fillFormat = categoryAxis.Area.FillFormat;

            // تعيين لون مسبق متدرج لتنسيق التعبئة
            fillFormat.SetPresetColorGradient(GradientPresetType.Fire, GradientStyleType.Horizontal, 1);

            // إخراج نوع اللون المسبق المتدرج
            Console.WriteLine("Gradient Preset Color: " + fillFormat.PresetColor);

            // احفظ المصنف
            workbook.Save("GradientPresetTypeExample.xlsx");
            workbook.Save("GradientPresetTypeExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


