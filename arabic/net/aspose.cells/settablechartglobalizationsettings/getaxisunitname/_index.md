---
title: "SettableChartGlobalizationSettings.GetAxisUnitName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SettableChartGlobalizationSettings. الحصول على اسم وحدة المحور"
type: docs
url: /ar/net/aspose.cells/settablechartglobalizationsettings/getaxisunitname/
---
## SettableChartGlobalizationSettings.GetAxisUnitName method

يحصل على اسم وحدة المحور.

```csharp
public override string GetAxisUnitName(DisplayUnitType type)
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetAxisUnitNameWithDisplayUnitTypeDemo
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

                // استدعِ GetAxisUnitName مع قيم مختلفة لـ DisplayUnitType
                string hundredsUnit = settings.GetAxisUnitName(DisplayUnitType.Hundreds);
                string thousandsUnit = settings.GetAxisUnitName(DisplayUnitType.Thousands);
                string millionsUnit = settings.GetAxisUnitName(DisplayUnitType.Millions);
                string percentageUnit = settings.GetAxisUnitName(DisplayUnitType.Percentage);

                // عرض النتائج
                Console.WriteLine($"Hundreds unit name: {hundredsUnit}");
                Console.WriteLine($"Thousands unit name: {thousandsUnit}");
                Console.WriteLine($"Millions unit name: {millionsUnit}");
                Console.WriteLine($"Percentage unit name: {percentageUnit}");

                // احفظ المصنف
                workbook.Save("GetAxisUnitNameDemo.xlsx");
                Console.WriteLine("GetAxisUnitName method called successfully. Workbook saved.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetAxisUnitName: {ex.Message}");
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


