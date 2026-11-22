---
title: "SettablePivotGlobalizationSettings.SetTextOfColumnLabels"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SettablePivotGlobalizationSettings. تحصل على نص تسمية Column Labels في PivotTable"
type: docs
url: /ar/net/aspose.cells/settablepivotglobalizationsettings/settextofcolumnlabels/
---
## SettablePivotGlobalizationSettings.SetTextOfColumnLabels method

يحصل على نص التسمية "Column Labels" في جدول المحور.

```csharp
public void SetTextOfColumnLabels(string text)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| نص | String | نص تسميات الأعمدة |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfColumnLabelsWithStringDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد (فقط للسياق)
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Demo Data");

            try
            {
                // إنشاء نسخة من SettablePivotGlobalizationSettings
                SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

                // تعيين نص مخصص لتسمية "Column Labels"
                string customColumnLabel = "My Column Headers";
                settings.SetTextOfColumnLabels(customColumnLabel);

                // استرجاع النص الحالي للتحقق من التغيير
                string currentLabel = settings.GetTextOfColumnLabels();
                Console.WriteLine($"Column Labels text is now: \"{currentLabel}\"");

                // حفظ المصنف (لا يلزم جدول محوري لهذا العرض)
                workbook.Save("SetTextOfColumnLabelsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfColumnLabels: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


