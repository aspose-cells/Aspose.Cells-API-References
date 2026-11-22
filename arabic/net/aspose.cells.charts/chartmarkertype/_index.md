---
title: "تعداد ChartMarkerType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Charts.ChartMarkerType. يمثل نمط العلامة في مخطط خطي أو مخطط مبعثر أو مخطط رادار"
type: docs
url: /ar/net/aspose.cells.charts/chartmarkertype/
---
## ChartMarkerType enumeration

يمثل نمط العلامة في مخطط خطي أو مخطط مبعثر أو مخطط راداري.

```csharp
public enum ChartMarkerType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Automatic | `0` | علامات تلقائية. |
| Circle | `1` | علامات دائرية. |
| Dash | `2` | علامات شريطية طويلة |
| Diamond | `3` | علامات على شكل ماسة. |
| Dot | `4` | علامات شريطية قصيرة. |
| None | `5` | بدون علامات. |
| SquarePlus | `6` | علامات مربعة مع علامة زائد. |
| Square | `7` | علامات مربعة. |
| SquareStar | `8` | علامات مربعة مع نجمة. |
| Triangle | `9` | علامات مثلثية. |
| SquareX | `10` | علامات مربعة مع X. |
| Picture | `11` | صورة |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class ChartMarkerTypeDemo
    {
        public static void ChartMarkerTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // أضف سلسلة البيانات إلى المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // الوصول إلى العلامة في السلسلة الأولى
            Marker marker = chart.NSeries[0].Marker;

            // تعيين نمط العلامة
            marker.MarkerStyle = ChartMarkerType.Circle;

            // تعيين حجم العلامة
            marker.MarkerSize = 10;

            // تعيين ألوان المقدمة والخلفية للعلامة
            marker.ForegroundColor = Color.Red;
            marker.BackgroundColor = Color.Yellow;

            // احفظ المصنف
            workbook.Save("ChartMarkerTypeExample.xlsx");
            workbook.Save("ChartMarkerTypeExample.pdf");
            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


