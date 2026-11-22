---
title: "Series.DataLabels"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Series. تمثل كائن DataLabels للسلسلة المحددة ASeries"
type: docs
url: /ar/net/aspose.cells.charts/series/datalabels/
---
## Series.DataLabels property

يمثل كائن DataLabels للسلسلة المحددة ASeries.

```csharp
public DataLabels DataLabels { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyDataLabelsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى وإضافة بيانات نموذجية
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Cells["A1"].PutValue("Products");
            dataSheet.Cells["B1"].PutValue("Users");
            dataSheet.Cells["A2"].PutValue("Aspose.Cells");
            dataSheet.Cells["B2"].PutValue(10000);
            dataSheet.Cells["A3"].PutValue("Aspose.Slides");
            dataSheet.Cells["B3"].PutValue(8000);
            dataSheet.Cells["A4"].PutValue("Aspose.Words");
            dataSheet.Cells["B4"].PutValue(12000);

            // إضافة ورقة مخطط وإنشاء مخطط فطيرة
            Worksheet chartSheet = workbook.Worksheets[workbook.Worksheets.Add(SheetType.Chart)];
            Chart chart = chartSheet.Charts[chartSheet.Charts.Add(ChartType.Pie, 7, 0, 20, 6)];

            // أضف بيانات السلسلة وقم بتكوين تسميات البيانات
            Series series = chart.NSeries[chart.NSeries.Add("=Sheet1!$B$2:$B$4", true)];
            series.XValues = "=Sheet1!$A$2:$A$4";
            
            // قم بتكوين خصائص DataLabels
            series.DataLabels.ShowValue = true;
            series.DataLabels.ShowCategoryName = true;
            series.DataLabels.ShowPercentage = true;
            series.DataLabels.LinkedSource = null; // Explicitly set to null

            // احفظ المصنف
            workbook.Save("SeriesPropertyDataLabelsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [DataLabels](../../datalabels/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


