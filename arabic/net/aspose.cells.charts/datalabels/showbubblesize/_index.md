---
title: "DataLabels.ShowBubbleSize"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DataLabels. تمثل سلوك عرض قيمة النسبة المئوية لتسمية البيانات في المخطط المحدد. صحيح يعرض قيمة النسبة المئوية. خطأ يخفي قيمة النسبة المئوية"
type: docs
url: /ar/net/aspose.cells.charts/datalabels/showbubblesize/
---
## DataLabels.ShowBubbleSize property

يمثل سلوك عرض قيمة النسبة المئوية لتسمية البيانات في مخطط محدد. صحيح يعرض قيمة النسبة المئوية. خطأ يخفي قيمة النسبة المئوية.

```csharp
public bool ShowBubbleSize { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyShowBubbleSizeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة لمخطط الفقاعات
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B1"].PutValue("Y");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["C1"].PutValue("Size");
            worksheet.Cells["C2"].PutValue(5);
            worksheet.Cells["C3"].PutValue(10);
            worksheet.Cells["C4"].PutValue(15);

            // إضافة مخطط فقاعات
            int chartIndex = worksheet.Charts.Add(ChartType.Bubble, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // إضافة سلسلة إلى المخطط
            int seriesIndex = chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // تعيين أحجام الفقاعات للسلسلة
            Series series = chart.NSeries[seriesIndex];
            series.BubbleSizes = "C2:C4";

            // الوصول إلى DataLabels الخاصة بالسلسلة
            DataLabels dataLabels = series.DataLabels;

            // عرض خاصية ShowBubbleSize
            dataLabels.ShowBubbleSize = true; // Show bubble size in data labels
            dataLabels.ShowValue = true;      // Also show values for clarity

            // احفظ المصنف
            workbook.Save("DataLabelsShowBubbleSizeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


