---
title: "ChartGlobalizationSettings.GetChartTitleName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ChartGlobalizationSettings. تحصل على اسم عنوان المخطط"
type: docs
url: /ar/net/aspose.cells.charts/chartglobalizationsettings/getcharttitlename/
---
## ChartGlobalizationSettings.GetChartTitleName method

يحصل على اسم عنوان المخطط.

```csharp
public virtual string GetChartTitleName()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartGlobalizationSettingsMethodGetChartTitleNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف مخططًا تجريبيًا إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["A3"].PutValue("Category 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // أنشئ نسخة من ChartGlobalizationSettings
            ChartGlobalizationSettings globalizationSettings = new ChartGlobalizationSettings();

            // عرض استخدام طريقة GetChartTitleName
            string chartTitleName = globalizationSettings.GetChartTitleName();
            Console.WriteLine("Chart Title Name: " + chartTitleName);

            // احفظ المصنف
            workbook.Save("ChartGlobalizationSettingsExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartGlobalizationSettings](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


