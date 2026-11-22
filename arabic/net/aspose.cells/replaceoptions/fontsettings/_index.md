---
title: "ReplaceOptions.FontSettings"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ReplaceOptions. إعدادات التنسيق الغني للنص المستبدل"
type: docs
url: /ar/net/aspose.cells/replaceoptions/fontsettings/
---
## ReplaceOptions.FontSettings property

إعدادات التنسيق الغني للنص المستبدل.

```csharp
public FontSetting[] FontSettings { get; set; }
```

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReplaceOptionsPropertyFontSettingsDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // حدد نصًا تجريبيًا في الخلية A1
            worksheet.Cells["A1"].Value = "Sample text for replacement";
            
            // إنشاء خيارات الاستبدال مع إعدادات الخط
            ReplaceOptions options = new ReplaceOptions();
            options.MatchEntireCellContents = false;
            
            // إنشاء إعداد خط للنص المستبدل
            FontSetting fontSetting = new FontSetting(0, 8, workbook.Worksheets);
            fontSetting.Font.IsBold = true;
            fontSetting.Font.Color = Color.Blue;
            
            // تطبيق إعدادات الخط على خيارات الاستبدال
            options.FontSettings = new FontSetting[] { fontSetting };
            
            // تنفيذ الاستبدال
            workbook.Replace("text", "REPLACED", options);
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [FontSetting](../../fontsetting/)
* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


