---
title: "SettableChartGlobalizationSettings.GetLegendIncreaseName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SettableChartGlobalizationSettings. تحصل على اسم الزيادة للوسيلة الإيضاحية"
type: docs
url: /ar/net/aspose.cells/settablechartglobalizationsettings/getlegendincreasename/
---
## SettableChartGlobalizationSettings.GetLegendIncreaseName method

يحصل على اسم الزيادة للوسيلة الإيضاحية.

```csharp
public override string GetLegendIncreaseName()
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetLegendIncreaseNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات قليلة للسياق
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // إنشاء نسخة من SettableChartGlobalizationSettings
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // حدد اسمًا مخصصًا للزيادة للوسيلة الإيضاحية
                settings.SetLegendIncreaseName("Custom Increase Label");

                // احصل على اسم الزيادة للوسيلة الإيضاحية باستخدام GetLegendIncreaseName
                string legendIncreaseName = settings.GetLegendIncreaseName();
                Console.WriteLine("Legend Increase Name: " + legendIncreaseName);

                // احفظ المصنف
                workbook.Save("GetLegendIncreaseNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetLegendIncreaseName: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


