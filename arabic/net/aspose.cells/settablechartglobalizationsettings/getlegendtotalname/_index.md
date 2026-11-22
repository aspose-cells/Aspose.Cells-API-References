---
title: "SettableChartGlobalizationSettings.GetLegendTotalName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SettableChartGlobalizationSettings. الحصول على اسم الإجمالي للوسيلة الإيضاحية"
type: docs
url: /ar/net/aspose.cells/settablechartglobalizationsettings/getlegendtotalname/
---
## SettableChartGlobalizationSettings.GetLegendTotalName method

يحصل على اسم الإجمالي للوسيلة الإيضاحية.

```csharp
public override string GetLegendTotalName()
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetLegendTotalNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات للسياق
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // إنشاء نسخة من SettableChartGlobalizationSettings
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // أولاً قم بتعيين اسم إجمالي مخصص للوسيلة الإيضاحية
                settings.SetLegendTotalName("Custom Total Label");

                // استدعِ طريقة GetLegendTotalName لاسترجاع القيمة
                string legendTotalName = settings.GetLegendTotalName();

                // اعرض النتيجة
                Console.WriteLine("Legend Total Name: " + legendTotalName);

                // احفظ المصنف
                workbook.Save("GetLegendTotalNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetLegendTotalName: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


