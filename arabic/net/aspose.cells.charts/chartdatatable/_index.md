---
title: "الفئة ChartDataTable"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Charts.ChartDataTable. تمثل جدول بيانات المخطط"
type: docs
url: /ar/net/aspose.cells.charts/chartdatatable/
---
## ChartDataTable class

يمثل جدول بيانات المخطط.

```csharp
public class ChartDataTable
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AutoScaleFont](../../aspose.cells.charts/chartdatatable/autoscalefont/) { get; set; } | صحيح إذا كان النص في الكائن يغيّر حجم الخط عندما يتغيّر حجم الكائن. القيمة الافتراضية هي True. |
| [BackgroundMode](../../aspose.cells.charts/chartdatatable/backgroundmode/) { get; set; } | يحصل ويضبط وضع عرض الخلفية. |
| [Border](../../aspose.cells.charts/chartdatatable/border/) { get; } | يعيد كائن Border الذي يمثل حد الكائن |
| [Font](../../aspose.cells.charts/chartdatatable/font/) { get; } | يحصل على كائن [`Font`](./font/) الذي يمثل إعداد الخط لجدول بيانات المخطط المحدد. |
| [HasBorderHorizontal](../../aspose.cells.charts/chartdatatable/hasborderhorizontal/) { get; set; } | (**Obsolete.**) صحيح إذا كان جدول بيانات المخطط يحتوي على حدود خلايا أفقية |
| [HasBorderOutline](../../aspose.cells.charts/chartdatatable/hasborderoutline/) { get; set; } | (**مهمل.**) صحيح إذا كان جدول بيانات المخطط يحتوي على حدود خارجية |
| [HasBorderVertical](../../aspose.cells.charts/chartdatatable/hasbordervertical/) { get; set; } | (**مهمل.**) صحيح إذا كان جدول بيانات المخطط يحتوي على حدود خلايا عمودية |
| [HasHorizontalBorder](../../aspose.cells.charts/chartdatatable/hashorizontalborder/) { get; set; } | صحيح إذا كان جدول بيانات المخطط يحتوي على حدود خلايا أفقية |
| [HasOutlineBorder](../../aspose.cells.charts/chartdatatable/hasoutlineborder/) { get; set; } | صحيح إذا كان جدول بيانات المخطط يحتوي على حدود خارجية |
| [HasVerticalBorder](../../aspose.cells.charts/chartdatatable/hasverticalborder/) { get; set; } | صحيح إذا كان جدول بيانات المخطط يحتوي على حدود خلايا عمودية |
| [ShowLegendKey](../../aspose.cells.charts/chartdatatable/showlegendkey/) { get; set; } | صحيح إذا كان مفتاح وسيلة إيضاح تسمية البيانات مرئياً. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class ChartDataTableDemo
    {
        public static void ChartDataTableExample()
        {
            // إنشاء كائن Workbook
            Workbook workbook = new Workbook();

            // الحصول على مرجع ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة قيم عينة إلى الخلايا
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);

            // الوصول إلى نسخة المخطط المضاف حديثًا
            Chart chart = worksheet.Charts[chartIndex];

            // إضافة NSeries (مصدر بيانات المخطط) إلى المخطط من الخلية "A1" إلى "B3"
            chart.NSeries.Add("A1:B3", true);

            // عرض جدول البيانات
            chart.ShowDataTable = true;

            // الحصول على جدول بيانات المخطط
            ChartDataTable chartTable = chart.ChartDataTable;

            // تعيين خصائص جدول بيانات المخطط
            chartTable.Font.Color = Color.Red;
            chartTable.AutoScaleFont = true;
            chartTable.BackgroundMode = BackgroundMode.Transparent;
            chartTable.HasBorderHorizontal = true;
            chartTable.HasBorderVertical = true;
            chartTable.HasBorderOutline = true;
            chartTable.ShowLegendKey = false;

            // حفظ ملف Excel
            workbook.Save("ChartDataTableExample.xlsx");
            workbook.Save("ChartDataTableExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


