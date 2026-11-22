---
title: "تعداد MapChartLabelLayout"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Charts.MapChartLabelLayout. يمثل تخطيط تسميات مخططات الخريطة"
type: docs
url: /ar/net/aspose.cells.charts/mapchartlabellayout/
---
## MapChartLabelLayout enumeration

يمثل تخطيط تسميات مخطط الخريطة.

```csharp
public enum MapChartLabelLayout
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| BestFitOnly | `0` | يتم استخدام الأنسب فقط. |
| ShowAll | `1` | يعرض جميع التسميات. |
| None | `2` | لا توجد تسميات. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class MapChartLabelLayoutDemo
    {
        public static void MapChartLabelLayoutExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة لمخطط الخريطة
            worksheet.Cells["A1"].PutValue("Country");
            worksheet.Cells["A2"].PutValue("USA");
            worksheet.Cells["A3"].PutValue("Canada");
            worksheet.Cells["A4"].PutValue("Mexico");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(150);

            // أضف مخطط خريطة إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Map, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // تحديد نطاق البيانات للمخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // الوصول إلى خصائص تخطيط السلسلة
            SeriesLayoutProperties layoutProperties = chart.NSeries[0].LayoutProperties;

            // تعيين تخطيط تسمية مخطط الخريطة
            layoutProperties.MapLabelLayout = MapChartLabelLayout.ShowAll;

            // احفظ المصنف
            workbook.Save("MapChartLabelLayoutExample.xlsx");

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


