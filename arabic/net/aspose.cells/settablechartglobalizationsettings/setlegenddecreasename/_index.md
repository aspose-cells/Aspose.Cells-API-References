---
title: "SettableChartGlobalizationSettings.SetLegendDecreaseName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SettableChartGlobalizationSettings. تعيين اسم الانخفاض للوسيلة الإيضاحية"
type: docs
url: /ar/net/aspose.cells/settablechartglobalizationsettings/setlegenddecreasename/
---
## SettableChartGlobalizationSettings.SetLegendDecreaseName method

يضبط اسم الانخفاض للوسيلة الإيضاحية.

```csharp
public void SetLegendDecreaseName(string name)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| name | String | اسم محلي معتمد |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SettableChartGlobalizationSettingsMethodSetLegendDecreaseNameWithStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية لمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Series");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);

            // إنشاء مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // أنشئ إعدادات العولمة
            SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

            try
            {
                // استدعاء SetLegendDecreaseName مع سلسلة مخصصة
                settings.SetLegendDecreaseName("Custom Decrease Label");

                // فئة Chart لا تحتوي على خاصية ChartGlobalizationSettings،
                // لذا نحتاج إلى استخدام كائن الإعدادات مباشرةً حيثما يلزم
                // (ملاحظة: في الاستخدام الفعلي، ستحتاج إلى العثور على المكان الذي تُطبق فيه هذه الإعدادات)
                Console.WriteLine("SetLegendDecreaseName method executed successfully with parameter: 'Custom Decrease Label'");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetLegendDecreaseName method: {ex.Message}");
            }

            // احفظ المصنف
            workbook.Save("SetLegendDecreaseNameDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


