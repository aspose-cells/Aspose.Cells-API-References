---
title: "Class DropBars"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Charts.DropBars. تمثل الأشرطة الصاعدة والهابطة في المخطط"
type: docs
url: /ar/net/aspose.cells.charts/dropbars/
---
## DropBars class

يمثل أشرطة الصعود والهبوط في المخطط.

```csharp
public class DropBars
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Area](../../aspose.cells.charts/dropbars/area/) { get; } | يحصل على [`Area`](./area/). |
| [Border](../../aspose.cells.charts/dropbars/border/) { get; } | يحصل على حد [`Line`](../../aspose.cells.drawing/line/). |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class DropBarsDemo
    {
        public static void DropBarsExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات التجريبية
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // أضف NSeries (مصدر بيانات المخطط) إلى المخطط من الخلية \"A1\" إلى \"B3\"
            chart.NSeries.Add("A1:B3", true);

            // تمكين الأشرطة الصاعدة والهابطة
            chart.NSeries[0].HasUpDownBars = true;

            // الوصول إلى كائن DropBars
            DropBars upBars = chart.NSeries[0].UpBars;
            DropBars downBars = chart.NSeries[0].DownBars;

            // تخصيص مظهر الأشرطة الصاعدة
            upBars.Border.Color = Color.Green;
            upBars.Area.ForegroundColor = Color.LightGreen;

            // تخصيص مظهر الأشرطة الهابطة
            downBars.Border.Color = Color.Red;
            downBars.Area.ForegroundColor = Color.LightCoral;

            // احفظ المصنف
            workbook.Save("DropBarsExample.xlsx");
            workbook.Save("DropBarsExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


