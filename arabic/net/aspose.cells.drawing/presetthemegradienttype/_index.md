---
title: "تعداد PresetThemeGradientType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Drawing.PresetThemeGradientType. يمثل نوع تدرج السمة المحدد مسبقًا"
type: docs
url: /ar/net/aspose.cells.drawing/presetthemegradienttype/
---
## PresetThemeGradientType enumeration

يمثل نوع تدرج السمة المسبق.

```csharp
public enum PresetThemeGradientType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| LightGradient | `0` | تدرج فاتح |
| TopSpotlight | `1` | إضاءة علوية |
| MediumGradient | `2` | تدرج متوسط |
| BottomSpotlight | `3` | إضاءة سفلية |
| RadialGradient | `4` | تدرج شعاعي |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DrawingClassPresetThemeGradientTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Category 1");
            worksheet.Cells["A3"].PutValue("Category 2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B3", true);

            // تطبيق تعبئة التدرج على السلسلة الأولى
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            series.Area.FillFormat.FillType = FillType.Gradient;
            series.Area.FillFormat.GradientFill.SetPresetThemeGradient(
                PresetThemeGradientType.RadialGradient, 
                ThemeColorType.Accent1);

            // احفظ المصنف
            workbook.Save("PresetThemeGradientDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


