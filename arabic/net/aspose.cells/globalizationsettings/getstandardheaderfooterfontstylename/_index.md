---
title: "GlobalizationSettings.GetStandardHeaderFooterFontStyleName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة GlobalizationSettings. يحصل على اسم نمط الخط الإنجليزي القياسي Regular Bold Italic للرأس/التذييل وفقًا لاسم نمط الخط المعطى للمنطقة"
type: docs
url: /ar/net/aspose.cells/globalizationsettings/getstandardheaderfooterfontstylename/
---
## GlobalizationSettings.GetStandardHeaderFooterFontStyleName method

يحصل على اسم نمط الخط الإنجليزي المعياري (Regular, Bold, Italic) للرأس/التذييل وفقًا لاسم نمط الخط المعتمد على اللغة المعطى.

```csharp
public virtual string GetStandardHeaderFooterFontStyleName(string localfontStyleName)
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

    public class GlobalizationSettingsMethodGetStandardHeaderFooterFontStyleNameWithStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء مثيل لإعدادات تعميم مخصصة
            var globalizationSettings = new CustomGlobalizationSettings();

            try
            {
                // عرض استدعاء الطريقة مع نوع المعامل (String)
                string localStyle = "CustomBold";
                string standardStyle = globalizationSettings.GetStandardHeaderFooterFontStyleName(localStyle);
                Console.WriteLine($"Converted font style: {localStyle} -> {standardStyle}");

                // تطبيق إعدادات التعميم على المصنف
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                // تعيين الرأس بنمط خط مخصص سيتم تحويله
                // استخدام طريقة SetHeader مع معامل القسم (0 = يسار، 1 = مركز، 2 = يمين)
                worksheet.PageSetup.SetHeader(1, "&\"Arial\"&\"CustomBold\"&12Header Text");

                // حفظ المصنف لإظهار التأثير
                workbook.Save("MethodGetStandardHeaderFooterFontStyleNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardHeaderFooterFontStyleName method: {ex.Message}");
            }
        }
    }

    // تنفيذ إعدادات التعريب المخصصة
    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetStandardHeaderFooterFontStyleName(string localfontStyleName)
        {
            // تحويل أسماء أنماط الخط المخصصة إلى أسماء قياسية
            return localfontStyleName switch
            {
                "CustomBold" => "Bold",
                "CustomItalic" => "Italic",
                _ => base.GetStandardHeaderFooterFontStyleName(localfontStyleName)
            };
        }
    }
}
```

### انظر أيضًا

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


