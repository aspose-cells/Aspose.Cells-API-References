---
title: "SettablePivotGlobalizationSettings.GetTextOfColumnLabels"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SettablePivotGlobalizationSettings. تحصل على نص تسمية Column Labels في PivotTable"
type: docs
url: /ar/net/aspose.cells/settablepivotglobalizationsettings/gettextofcolumnlabels/
---
## SettablePivotGlobalizationSettings.GetTextOfColumnLabels method

يحصل على نص التسمية "Column Labels" في جدول المحور.

```csharp
public override string GetTextOfColumnLabels()
```

### قيمة الإرجاع

نص تسميات الأعمدة

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfColumnLabelsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة للسياق
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            // إنشاء نسخة من SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // احصل على النص الافتراضي لتسميات الأعمدة
                string columnLabelsText = settings.GetTextOfColumnLabels();
                Console.WriteLine($"Default text of Column Labels: {columnLabelsText}");

                // تعيين نص مخصص لتسميات الأعمدة
                settings.SetTextOfColumnLabels("Custom Column Headers");

                // احصل على النص المحدث لتسميات الأعمدة
                string updatedColumnLabelsText = settings.GetTextOfColumnLabels();
                Console.WriteLine($"Updated text of Column Labels: {updatedColumnLabelsText}");

                // احفظ المصنف
                workbook.Save("GetTextOfColumnLabelsDemo.xlsx");
                Console.WriteLine("GetTextOfColumnLabels method executed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfColumnLabels: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


