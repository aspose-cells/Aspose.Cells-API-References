---
title: "ChartGlobalizationSettings.GetLegendTotalName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ChartGlobalizationSettings. تحصل على اسم الإجمالي للوسيلة الإيضاحية"
type: docs
url: /ar/net/aspose.cells.charts/chartglobalizationsettings/getlegendtotalname/
---
## ChartGlobalizationSettings.GetLegendTotalName method

يحصل على اسم الإجمالي للوسيلة الإيضاحية.

```csharp
public virtual string GetLegendTotalName()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartGlobalizationSettingsMethodGetLegendTotalNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // إنشاء إعدادات العولمة والحصول على اسم إجمالي الوسيلة الإيضاحية
            ChartGlobalizationSettings globalizationSettings = new ChartGlobalizationSettings();
            string legendTotalName = globalizationSettings.GetLegendTotalName();

            // أخرج النتيجة.
            Console.WriteLine("Legend Total Name: " + legendTotalName);

            // احفظ دفتر العمل
            workbook.Save("ChartGlobalizationDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartGlobalizationSettings](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


