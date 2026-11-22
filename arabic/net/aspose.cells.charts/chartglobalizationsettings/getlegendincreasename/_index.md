---
title: "ChartGlobalizationSettings.GetLegendIncreaseName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ChartGlobalizationSettings. تحصل على اسم الزيادة للوسيلة الإيضاحية"
type: docs
url: /ar/net/aspose.cells.charts/chartglobalizationsettings/getlegendincreasename/
---
## ChartGlobalizationSettings.GetLegendIncreaseName method

يحصل على اسم الزيادة للوسيلة الإيضاحية.

```csharp
public virtual string GetLegendIncreaseName()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartGlobalizationSettingsMethodGetLegendIncreaseNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف مخططًا تجريبيًا
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // إنشاء إعدادات العولمة والحصول على اسم زيادة الوسيلة الإيضاحية
            ChartGlobalizationSettings globalizationSettings = new ChartGlobalizationSettings();
            string legendIncreaseName = globalizationSettings.GetLegendIncreaseName();

            // أخرج النتيجة.
            Console.WriteLine("Legend Increase Name: " + legendIncreaseName);

            // احفظ المصنف
            workbook.Save("ChartGlobalizationDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartGlobalizationSettings](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


