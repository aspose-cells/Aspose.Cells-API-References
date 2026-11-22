---
title: "تعداد PlotEmptyCellsType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Charts.PlotEmptyCellsType. يمثل جميع أنواع خلايا الرسم الفارغة في المخطط"
type: docs
url: /ar/net/aspose.cells.charts/plotemptycellstype/
---
## PlotEmptyCellsType enumeration

يمثل جميع أنواع الخلايا الفارغة في رسم المخطط.

```csharp
public enum PlotEmptyCellsType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| NotPlotted | `0` | غير مرسوم (اترك فجوة) |
| Zero | `1` | صفر |
| Interpolated | `2` | مُستَدل |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PlotEmptyCellsTypeDemo
    {
        public static void PlotEmptyCellsTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات التجريبية
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(null); // Empty cell
            worksheet.Cells["A5"].PutValue("D");
            worksheet.Cells["B5"].PutValue(40);

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 7, 1, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // تحديد نطاق البيانات للمخطط
            chart.SetChartDataRange("A1:B5", true);

            // تحديد عنوان المخطط
            chart.Title.Text = "Plot Empty Cells Example";

            // حدد كيفية رسم الخلايا الفارغة
            chart.PlotEmptyCellsType = PlotEmptyCellsType.Interpolated;

            // احفظ المصنف
            workbook.Save("PlotEmptyCellsTypeExample.xlsx");

            Console.WriteLine("Workbook saved successfully.");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


