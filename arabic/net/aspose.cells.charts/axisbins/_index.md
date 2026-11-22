---
title: "الفئة AxisBins"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Charts.AxisBins. تمثّل حاويات المحور"
type: docs
url: /ar/net/aspose.cells.charts/axisbins/
---
## AxisBins class

يمثل فواصل المحور.

```csharp
public class AxisBins
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Count](../../aspose.cells.charts/axisbins/count/) { get; set; } | يحصل أو يعيّن عدد حاويات المحور |
| [IsAutomatic](../../aspose.cells.charts/axisbins/isautomatic/) { get; set; } | يشير إلى ما إذا كانت حاويات المحور تلقائية. |
| [IsByCategory](../../aspose.cells.charts/axisbins/isbycategory/) { get; set; } | يشير إلى ما إذا كان تجميع البيانات حسب الفئة مفعّلاً. |
| [Overflow](../../aspose.cells.charts/axisbins/overflow/) { get; set; } | يحصل أو يعيّن الفائض لحاويات المحور |
| [Underflow](../../aspose.cells.charts/axisbins/underflow/) { get; set; } | يحصل أو يعيّن النقص لحاويات المحور |
| [Width](../../aspose.cells.charts/axisbins/width/) { get; set; } | يحصل أو يعيّن عرض حاوية المحور. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [ResetOverflow](../../aspose.cells.charts/axisbins/resetoverflow/)() | (**Obsolete.**) إعادة تعيين الفائض |
| [ResetUnderflow](../../aspose.cells.charts/axisbins/resetunderflow/)() | (**Obsolete.**) إعادة تعيين النقص |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class AxisBinsDemo
    {
        public static void AxisBinsExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            // إضافة ورقة عمل جديدة
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات التجريبية
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Histogram, 5, 0, 25, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // إضافة سلسلة بيانات إلى المخطط.
            chart.NSeries.Add("A1:A5", true);

            // الوصول إلى محور القيم
            Axis valueAxis = chart.ValueAxis;

            // الوصول إلى حاويات محور القيم
            AxisBins bins = valueAxis.Bins;

            // تعيين الخصائص للحاويات
            bins.IsByCategory = false;
            bins.IsAutomatic = true;
            bins.Width = 10.0;
            bins.Count = 5;
            bins.Overflow = 60.0;
            bins.Underflow = 0.0;

            // إعادة تعيين الفائض والنقص
            //bins.ResetOverflow();
            //bins.ResetUnderflow();

            // احفظ المصنف
            workbook.Save("AxisBinsExample.xlsx");
            workbook.Save("AxisBinsExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


