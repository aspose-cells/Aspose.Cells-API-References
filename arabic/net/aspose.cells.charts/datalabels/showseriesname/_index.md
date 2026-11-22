---
title: "DataLabels.ShowSeriesName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DataLabels. تشير إلى ما إذا كان اسم السلسلة يُعرض على تسميات البيانات في المخطط. true لإظهار اسم السلسلة. false لإخفائه"
type: docs
url: /ar/net/aspose.cells.charts/datalabels/showseriesname/
---
## DataLabels.ShowSeriesName property

يشير إلى ما إذا كان اسم السلسلة يُعرض على تسميات البيانات في المخطط. صحيح لإظهار اسم السلسلة. خطأ لإخفائه.

```csharp
public bool ShowSeriesName { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyShowSeriesNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Series 1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["B1"].PutValue("Series 2");
            worksheet.Cells["B2"].PutValue(15);
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(35);

            // أضف مخطط عمودي
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("A1:A4", true);
            chart.NSeries.Add("B1:B4", true);

            // تفعيل تسميات البيانات للسلسلة الأولى
            Series series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;

            // تفعيل إظهار اسم السلسلة لتسمية البيانات للنقطة المحددة
            var points = series.Points;
            points[1].DataLabels.ShowSeriesName = true;

            // حساب المخطط
            chart.Calculate();

            // احفظ المصنف
            workbook.Save("DataLabelsShowSeriesNameDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


