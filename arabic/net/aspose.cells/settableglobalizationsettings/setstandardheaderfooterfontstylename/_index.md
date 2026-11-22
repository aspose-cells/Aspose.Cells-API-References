---
title: "SettableGlobalizationSettings.SetStandardHeaderFooterFontStyleName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SettableGlobalizationSettings. تعيين اسم الدالة المعتمد على الإعدادات المحلية وفقًا لاسم الدالة القياسي المعطى"
type: docs
url: /ar/net/aspose.cells/settableglobalizationsettings/setstandardheaderfooterfontstylename/
---
## SettableGlobalizationSettings.SetStandardHeaderFooterFontStyleName method

يضبط اسم الدالة المعتمد على الإعدادات الإقليمية وفقًا لاسم الدالة القياسي المعطى.

```csharp
public void SetStandardHeaderFooterFontStyleName(string localfontStyleName, string standardName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| localfontStyleName | String | اسم نمط الخط المحلي للترويسة/التذييل. |
| standardName | String | اسم الدالة القياسي (إعداد محلي en-US). |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetStandardHeaderFooterFontStyleNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء خيارات إعداد الصفحة لورقة العمل
            PageSetup pageSetup = worksheet.PageSetup;

            // تعيين رأس يحتوي على بعض النص
            pageSetup.SetHeader(0, "&\"Arial\"&12This is a header");

            // إنشاء مثال لإعدادات العولمة
            SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();

            try
            {
                // استدعِ طريقة SetStandardHeaderFooterFontStyleName
                globalizationSettings.SetStandardHeaderFooterFontStyleName("Arial", "Times New Roman");

                // تطبيق إعدادات العولمة على دفتر العمل
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                Console.WriteLine("SetStandardHeaderFooterFontStyleName method executed successfully with parameters (\"Arial\", \"Times New Roman\")");

                // سيكون التأثير مرئياً عندما يتم عرض المستند أو طباعته
                // سيتم اعتبار نمط الخط "Arial" في الرؤوس/التذييلات كـ "Times New Roman"
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetStandardHeaderFooterFontStyleName method: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("MethodSetStandardHeaderFooterFontStyleNameDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


