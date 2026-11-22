---
title: "SettableGlobalizationSettings.GetStandardHeaderFooterFontStyleName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SettableGlobalizationSettings. تحصل على اسم نمط الخط الإنجليزي القياسي (عادي، عريض، مائل) للترويسة/التذييل وفقًا لاسم نمط الخط المحلي المعطى"
type: docs
url: /ar/net/aspose.cells/settableglobalizationsettings/getstandardheaderfooterfontstylename/
---
## SettableGlobalizationSettings.GetStandardHeaderFooterFontStyleName method

يحصل على اسم نمط الخط الإنجليزي المعياري (Regular, Bold, Italic) للرأس/التذييل وفقًا لاسم نمط الخط المعتمد على اللغة المعطى.

```csharp
public override string GetStandardHeaderFooterFontStyleName(string localfontStyleName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| localfontStyleName | String | اسم نمط الخط المحلي للترويسة/التذييل. |

### قيمة الإرجاع

اسم نمط الخط الإنجليزي القياسي (عادي، عريض، مائل)

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetStandardHeaderFooterFontStyleNameWithStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء إعدادات تعميم مخصصة
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // تعيين ربط اسم نمط خط الترويسة/التذييل القياسي
            settings.SetStandardHeaderFooterFontStyleName("MyLocalFontStyle", "Arial");

            // طبق الإعدادات على المصنف
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // استدعِ طريقة GetStandardHeaderFooterFontStyleName باستخدام اسم نمط خط محلي
                string standardFontStyle = settings.GetStandardHeaderFooterFontStyleName("MyLocalFontStyle");
                
                // اعرض النتيجة
                Console.WriteLine($"Standard font style name for 'MyLocalFontStyle': {standardFontStyle}");

                // إنشاء ترويسة باستخدام اسم نمط الخط المحلي
                worksheet.PageSetup.SetHeader(1, "&\"MyLocalFontStyle\"&12Test Header");

                // عرض التأثير في جدول البيانات
                Console.WriteLine("Header set with local font style name 'MyLocalFontStyle'");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardHeaderFooterFontStyleName method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("MethodGetStandardHeaderFooterFontStyleNameDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


