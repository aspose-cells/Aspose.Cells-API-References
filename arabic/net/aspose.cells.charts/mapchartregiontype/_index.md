---
title: "Enum MapChartRegionType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Charts.MapChartRegionType enum. يمثل نوع المنطقة في مخطط الخريطة"
type: docs
url: /ar/net/aspose.cells.charts/mapchartregiontype/
---
## MapChartRegionType enumeration

يمثل نوع المنطقة لمخطط الخريطة.

```csharp
public enum MapChartRegionType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Automatic | `0` | تلقائي |
| DataOnly | `1` | يحتوي على البيانات فقط. |
| CountryRegionList | `2` | قائمة مناطق الدول. |
| World | `3` | العالم. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class MapChartRegionTypeDemo
    {
        public static void MapChartRegionTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إضافة ورقة عمل جديدة إلى المصنف
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Country");
            worksheet.Cells["A2"].PutValue("USA");
            worksheet.Cells["A3"].PutValue("Canada");
            worksheet.Cells["A4"].PutValue("Mexico");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);

            // أضف مخطط خريطة إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Map, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين نطاق بيانات المخطط
            chart.SetChartDataRange("A1:B4", true);

            // تعيين نوع المنطقة في مخطط الخريطة
            foreach (Series series in chart.NSeries)
            {
                series.LayoutProperties.MapChartRegionType = MapChartRegionType.CountryRegionList;
            }

            // احفظ المصنف
            workbook.Save("MapChartRegionTypeExample.xlsx");

            // أخرج النتيجة.
            Console.WriteLine("Map chart with region type 'CountryRegionList' created successfully.");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


