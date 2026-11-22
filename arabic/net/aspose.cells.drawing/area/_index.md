---
title: "الفئة Area"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Drawing.Area. تغلف الكائن الذي يمثل تنسيق المنطقة"
type: docs
url: /ar/net/aspose.cells.drawing/area/
---
## Area class

يغلف الكائن الذي يمثل تنسيق المنطقة.

```csharp
public class Area
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [BackgroundColor](../../aspose.cells.drawing/area/backgroundcolor/) { get; set; } | يحصل أو يضبط لون الخلفية لـ `Area`. |
| [FillFormat](../../aspose.cells.drawing/area/fillformat/) { get; } | يمثل كائن [`FillFormat`](./fillformat/) يحتوي على خصائص تنسيق التعبئة للمخطط أو الشكل المحدد. |
| [ForegroundColor](../../aspose.cells.drawing/area/foregroundcolor/) { get; set; } | الحصول على أو تعيين لون الأمام. |
| [Formatting](../../aspose.cells.drawing/area/formatting/) { get; set; } | يمثل تنسيق المنطقة. |
| [InvertIfNegative](../../aspose.cells.drawing/area/invertifnegative/) { get; set; } | إذا كانت الخاصية صحيحة وكانت قيمة نقطة المخطط عددًا سالبًا، سيتم تبادل لون المقدمة ولون الخلفية. |
| [Transparency](../../aspose.cells.drawing/area/transparency/) { get; set; } | يعيد أو يضبط درجة شفافية المنطقة كقيمة من 0.0 (معتم) إلى 1.0 (شفاف). |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class AreaDemo
    {
        public static void AreaExample()
        {
            // إنشاء كائن Workbook
            Workbook workbook = new Workbook();
            // إضافة ورقة عمل جديدة إلى كائن Workbook
            int sheetIndex = workbook.Worksheets.Add();
            // الحصول على مرجع ورقة العمل التي تم إضافتها حديثًا بتمرير sheet index
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            // إضافة قيم عينة إلى الخلايا
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(-100);
            worksheet.Cells["A3"].PutValue(150);
            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Area, 5, 0, 15, 5);
            // الوصول إلى نسخة المخطط المضاف حديثًا
            Chart chart = worksheet.Charts[chartIndex];
            // إضافة NSeries (مصدر بيانات المخطط) إلى المخطط من الخلية "A1" إلى "A3"
            chart.NSeries.Add("A1:A3", true);

            // الوصول إلى منطقة أول NSeries
            Area area = chart.NSeries[0].Area;

            // ضبط الخصائص
            area.InvertIfNegative = true;
            area.ForegroundColor = Color.Red;
            area.BackgroundColor = Color.Yellow;
            area.Formatting = Aspose.Cells.Charts.FormattingType.Custom;
            area.Transparency = 0.5;

            // حفظ ملف Excel
            workbook.Save("AreaExample.xlsx");
            workbook.Save("AreaExample.pdf");

        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


