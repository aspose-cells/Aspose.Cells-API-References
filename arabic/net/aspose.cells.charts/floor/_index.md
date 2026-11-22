---
title: "الفئة Floor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Charts.Floor. تغلف الكائن الذي يمثل أرضية مخطط ثلاثي الأبعاد"
type: docs
url: /ar/net/aspose.cells.charts/floor/
---
## Floor class

يحتوي على الكائن الذي يمثل قاعدة المخطط ثلاثي الأبعاد.

```csharp
public class Floor : Area
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [BackgroundColor](../../aspose.cells.drawing/area/backgroundcolor/) { get; set; } | يحصل أو يضبط لون الخلفية للـ [`Area`](../../aspose.cells.drawing/area/). (موروث من [`Area`](../../aspose.cells.drawing/area/).) |
| [Border](../../aspose.cells.charts/floor/border/) { get; set; } | يحصل أو يضبط حد الـ [`Line`](../../aspose.cells.drawing/line/). |
| [FillFormat](../../aspose.cells.drawing/area/fillformat/) { get; } | يمثل كائن [`FillFormat`](../../aspose.cells.drawing/area/fillformat/) الذي يحتوي على خصائص تنسيق التعبئة للمخطط أو الشكل المحدد. (موروث من [`Area`](../../aspose.cells.drawing/area/).) |
| [ForegroundColor](../../aspose.cells.drawing/area/foregroundcolor/) { get; set; } | يحصل أو يضبط لون المقدمة. (موروث من [`Area`](../../aspose.cells.drawing/area/).) |
| [Formatting](../../aspose.cells.drawing/area/formatting/) { get; set; } | يمثل تنسيق المنطقة. (موروث من [`Area`](../../aspose.cells.drawing/area/).) |
| [InvertIfNegative](../../aspose.cells.drawing/area/invertifnegative/) { get; set; } | إذا كانت الخاصية true وكانت قيمة نقطة المخطط رقمًا سالبًا، سيتم تبادل لون المقدمة ولون الخلفية. (موروث من [`Area`](../../aspose.cells.drawing/area/).) |
| [Transparency](../../aspose.cells.drawing/area/transparency/) { get; set; } | يرجع أو يضبط درجة شفافية المنطقة كقيمة من 0.0 (معتم) إلى 1.0 (شفاف). (موروث من [`Area`](../../aspose.cells.drawing/area/).) |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class FloorDemo
    {
        public static void FloorExample()
        {
            // إنشاء كائن دفتر العمل
            Workbook workbook = new Workbook();

            // احصل على مجموعة الخلايا
            Cells cells = workbook.Worksheets[0].Cells;

            // ضع القيم في الخلايا
            cells["A1"].PutValue(1);
            cells["A2"].PutValue(2);
            cells["A3"].PutValue(3);

            // احصل على مجموعة المخططات
            ChartCollection charts = workbook.Worksheets[0].Charts;

            // أضف مخططًا جديدًا
            int index = charts.Add(ChartType.Column3DStacked, 5, 0, 15, 5);

            // احصل على المخطط المضاف حديثًا
            Chart chart = charts[index];

            // تعيين nseries للمخطط
            chart.NSeries.Add("A1:A3", true);

            // إظهار تسميات البيانات
            chart.NSeries[0].DataLabels.ShowValue = true;

            // الحصول على أرضية المخطط
            Floor floor = chart.Floor;

            // تعيين حد الأرضية باللون الأحمر
            floor.Border.Color = Color.Red;

            // تعيين تنسيق التعبئة
            floor.FillFormat.SetPresetColorGradient(GradientPresetType.CalmWater, GradientStyleType.DiagonalDown, 2);

            // عيّن الخصائص الإضافية
            floor.BackgroundColor = Color.LightBlue;
            floor.ForegroundColor = Color.DarkBlue;
            floor.Formatting = FormattingType.Custom;
            floor.InvertIfNegative = true;
            floor.Transparency = 0.5;

            // حفظ الملف
            workbook.Save(@"FloorExample.xlsx");
            workbook.Save(@"FloorExample.pdf");
        }
    }
}
```

### انظر أيضًا

* class [Area](../../aspose.cells.drawing/area/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


