---
title: "تعداد MapChartProjectionType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Charts.MapChartProjectionType. يمثل نوع الإسقاط لمخطط الخريطة"
type: docs
url: /ar/net/aspose.cells.charts/mapchartprojectiontype/
---
## MapChartProjectionType enumeration

يمثل نوع الإسقاط لمخطط الخريطة.

```csharp
public enum MapChartProjectionType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Automatic | `0` | تلقائي |
| Mercator | `1` | ميركاتور |
| Miller | `2` | ميلر |
| Albers | `3` | آلبيرس |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class MapChartProjectionTypeDemo
    {
        public static void MapChartProjectionTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إضافة ورقة عمل جديدة إلى المصنف
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات عينة إلى ورقة العمل لمخطط الخريطة
            worksheet.Cells["A1"].PutValue("Country");
            worksheet.Cells["A2"].PutValue("USA");
            worksheet.Cells["A3"].PutValue("Canada");
            worksheet.Cells["A4"].PutValue("Mexico");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(80);
            worksheet.Cells["B4"].PutValue(60);

            // أضف مخطط خريطة إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Map, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين نطاق بيانات المخطط
            chart.SetChartDataRange("A1:B4", true);

            // حدد نوع الإسقاط لمخطط الخريطة
            chart.NSeries[0].LayoutProperties.MapChartProjectionType = MapChartProjectionType.Mercator;

            // أخرج نوع الإسقاط
            Console.WriteLine("Map Chart Projection Type: " + chart.NSeries[0].LayoutProperties.MapChartProjectionType);

            // احفظ المصنف
            workbook.Save("MapChartProjectionTypeExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


