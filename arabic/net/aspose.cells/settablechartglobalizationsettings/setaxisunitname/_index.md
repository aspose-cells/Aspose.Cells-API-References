---
title: "SettableChartGlobalizationSettings.SetAxisUnitName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SettableChartGlobalizationSettings. تعيين اسم وحدة المحور"
type: docs
url: /ar/net/aspose.cells/settablechartglobalizationsettings/setaxisunitname/
---
## SettableChartGlobalizationSettings.SetAxisUnitName method

يضبط اسم وحدة المحور.

```csharp
public void SetAxisUnitName(DisplayUnitType type, string name)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| type | DisplayUnitType | نوع الوحدة لعرض تسميات المحور. |
| name | String | اسم محلي معتمد |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SettableChartGlobalizationSettingsMethodSetAxisUnitNameWithDisplayUnitTypeStringDemo
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

                // تعيين أسماء وحدة محور مخصصة لأنواع عرض الوحدة المختلفة
                settings.SetAxisUnitName(DisplayUnitType.Thousands, "K");
                settings.SetAxisUnitName(DisplayUnitType.Millions, "M");
                settings.SetAxisUnitName(DisplayUnitType.Percentage, "Pct");

                // تحقق من الإعدادات عن طريق استرجاع القيم
                string thousandsUnit = settings.GetAxisUnitName(DisplayUnitType.Thousands);
                string millionsUnit = settings.GetAxisUnitName(DisplayUnitType.Millions);
                string percentageUnit = settings.GetAxisUnitName(DisplayUnitType.Percentage);

                // عرض النتائج
                Console.WriteLine($"Thousands unit name set to: {thousandsUnit}");
                Console.WriteLine($"Millions unit name set to: {millionsUnit}");
                Console.WriteLine($"Percentage unit name set to: {percentageUnit}");

                // احفظ المصنف
                workbook.Save("SetAxisUnitNameDemo.xlsx");
                Console.WriteLine("SetAxisUnitName method called successfully. Workbook saved.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetAxisUnitName: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* enum [DisplayUnitType](../../../aspose.cells.charts/displayunittype/)
* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


