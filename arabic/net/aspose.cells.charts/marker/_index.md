---
title: "فئة Marker"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Charts.Marker. تمثل العلامة في مخطط خطي أو مخطط مبعثر أو مخطط راداري"
type: docs
url: /ar/net/aspose.cells.charts/marker/
---
## Marker class

يمثل العلامة في مخطط خطي أو مخطط مبعثر أو مخطط رادار.

```csharp
public class Marker
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Area](../../aspose.cells.charts/marker/area/) { get; } | يحصل على [`area`](./area/). |
| [BackgroundColor](../../aspose.cells.charts/marker/backgroundcolor/) { get; set; } | يمثل لون خلفية العلامة في مخطط خطي أو مخطط مبعثر أو مخطط راداري. |
| [BackgroundColorSetType](../../aspose.cells.charts/marker/backgroundcolorsettype/) { get; set; } | يحصل على أو يعيّن نوع مجموعة لون خلفية العلامة. |
| [Border](../../aspose.cells.charts/marker/border/) { get; } | يحصل على [`border`](../../aspose.cells.drawing/line/). |
| [ForegroundColor](../../aspose.cells.charts/marker/foregroundcolor/) { get; set; } | يمثل لون مقدمة العلامة في مخطط خطي أو مخطط مبعثر أو مخطط راداري. |
| [ForegroundColorSetType](../../aspose.cells.charts/marker/foregroundcolorsettype/) { get; set; } | يحصل أو يضبط نوع مجموعة لون المقدمة للعلامة. |
| [MarkerSize](../../aspose.cells.charts/marker/markersize/) { get; set; } | يمثل حجم العلامة بوحدة النقاط. ينطبق على مخطط خط، مخطط مبعثر، أو مخطط رادار. |
| [MarkerSizePx](../../aspose.cells.charts/marker/markersizepx/) { get; set; } | يمثل حجم العلامة بوحدات البكسل. ينطبق على مخططات الخط، المخططات المبعثرة، أو مخططات الرادار. |
| [MarkerStyle](../../aspose.cells.charts/marker/markerstyle/) { get; set; } | يمثل نمط العلامة. ينطبق على مخطط خط، مخطط مبعثر، أو مخطط رادار. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MarkerDemo
    {
        public static void MarkerExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            // احصل على مرجع ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية إلى الخلايا
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

            // الوصول إلى السلسلة الأولى
            Series series = chart.NSeries[0];

            // تعيين خصائص العلامة
            series.Marker.MarkerStyle = ChartMarkerType.Circle;
            series.Marker.MarkerSize = 10; // Size in points
            series.Marker.MarkerSizePx = 20; // Size in pixels
            series.Marker.ForegroundColor = Color.Red;
            series.Marker.ForegroundColorSetType = FormattingType.Custom;
            series.Marker.BackgroundColor = Color.Yellow;
            series.Marker.BackgroundColorSetType = FormattingType.Custom;

            // احفظ المصنف
            workbook.Save("MarkerExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


