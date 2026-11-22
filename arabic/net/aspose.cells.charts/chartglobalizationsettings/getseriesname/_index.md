---
title: "ChartGlobalizationSettings.GetSeriesName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ChartGlobalizationSettings. يحصل على اسم السلسلة في المخطط"
type: docs
url: /ar/net/aspose.cells.charts/chartglobalizationsettings/getseriesname/
---
## ChartGlobalizationSettings.GetSeriesName method

يحصل على اسم السلسلة في المخطط.

```csharp
public virtual string GetSeriesName()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartGlobalizationSettingsMethodGetSeriesNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["A3"].PutValue("Category 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // أضف مخططًا وقم بتعيين البيانات
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // إنشاء إعدادات العولمة والحصول على اسم السلسلة
            Aspose.Cells.Charts.ChartGlobalizationSettings globalizationSettings = new Aspose.Cells.Charts.ChartGlobalizationSettings();
            string seriesName = globalizationSettings.GetSeriesName();

            // أخرج النتيجة.
            Console.WriteLine("Series Name: " + seriesName);

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


