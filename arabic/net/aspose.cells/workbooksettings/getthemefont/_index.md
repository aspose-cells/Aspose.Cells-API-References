---
title: "WorkbookSettings.GetThemeFont"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة WorkbookSettings. يحصل على اسم خط السمة الافتراضي"
type: docs
url: /ar/net/aspose.cells/workbooksettings/getthemefont/
---
## WorkbookSettings.GetThemeFont method

يحصل على اسم خط السمة الافتراضي.

```csharp
public string GetThemeFont(FontSchemeType type)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| type | FontSchemeType | نوع مخطط الخط. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsMethodGetThemeFontWithFontSchemeTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // احصل على خط السمة الافتراضي لنوع المخطط الصغير
            string minorFont = workbook.Settings.GetThemeFont(FontSchemeType.Minor);
            Console.WriteLine("Minor theme font: " + minorFont);
            
            // احصل على خط السمة الافتراضي لنوع المخطط الكبير
            string majorFont = workbook.Settings.GetThemeFont(FontSchemeType.Major);
            Console.WriteLine("Major theme font: " + majorFont);
            
            // احفظ المصنف
            workbook.Save("ThemeFontExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [FontSchemeType](../../fontschemetype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


