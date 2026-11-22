---
title: "SettablePivotGlobalizationSettings.GetTextOfEmptyData"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SettablePivotGlobalizationSettings. تحصل على نص التسمية الفارغة في PivotTable"
type: docs
url: /ar/net/aspose.cells/settablepivotglobalizationsettings/gettextofemptydata/
---
## SettablePivotGlobalizationSettings.GetTextOfEmptyData method

يحصل على نص التسمية "(blank)" في جدول المحور.

```csharp
public override string GetTextOfEmptyData()
```

### قيمة الإرجاع

نص البيانات الفارغة

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfEmptyDataDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إنشاء نسخة من SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // احصل على النص الافتراضي للبيانات الفارغة
                string emptyDataText = settings.GetTextOfEmptyData();
                Console.WriteLine($"Default text for empty data: '{emptyDataText}'");

                // تعيين نص مخصص للبيانات الفارغة
                settings.SetTextOfEmptyData("No Data Available");

                // احصل على النص المحدث للبيانات الفارغة
                string updatedEmptyDataText = settings.GetTextOfEmptyData();
                Console.WriteLine($"Updated text for empty data: '{updatedEmptyDataText}'");

                // تطبيق الإعدادات على دفتر العمل
                SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();
                globalizationSettings.PivotSettings = settings;
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                // احفظ المصنف
                workbook.Save("GetTextOfEmptyDataDemo.xlsx");
                Console.WriteLine("GetTextOfEmptyData method demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating GetTextOfEmptyData: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


