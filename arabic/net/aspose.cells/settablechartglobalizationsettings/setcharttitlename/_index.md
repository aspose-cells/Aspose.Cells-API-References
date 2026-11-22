---
title: "SettableChartGlobalizationSettings.SetChartTitleName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SettableChartGlobalizationSettings. تحدد اسم عنوان المخطط"
type: docs
url: /ar/net/aspose.cells/settablechartglobalizationsettings/setcharttitlename/
---
## SettableChartGlobalizationSettings.SetChartTitleName method

يضبط اسم عنوان المخطط.

```csharp
public void SetChartTitleName(string name)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| name | String | اسم محلي معتمد |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableChartGlobalizationSettingsMethodSetChartTitleNameDemo
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

                // استدعِ SetChartTitleName بسلسلة مخصصة
                settings.SetChartTitleName("Custom Chart Title");

                // تحقق من الإعداد عن طريق الحصول على القيمة
                string chartTitleName = settings.GetChartTitleName();
                Console.WriteLine("Chart Title Name set to: " + chartTitleName);

                // احفظ المصنف
                workbook.Save("SetChartTitleNameDemo.xlsx");
                Console.WriteLine("SetChartTitleName method called successfully. Workbook saved.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetChartTitleName: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


