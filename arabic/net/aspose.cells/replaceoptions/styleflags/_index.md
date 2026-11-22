---
title: "ReplaceOptions.StyleFlags"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ReplaceOptions. يحصل على ويضبط أعلام تطبيق إعدادات الخط"
type: docs
url: /ar/net/aspose.cells/replaceoptions/styleflags/
---
## ReplaceOptions.StyleFlags property

يحصل على ويضبط علامات تطبيق إعدادات الخط.

```csharp
public StyleFlag[] StyleFlags { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ReplaceOptionsPropertyStyleFlagsDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة نص عينة إلى الخلية
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("test text");

            // إنشاء خيارات الاستبدال
            ReplaceOptions options = new ReplaceOptions();
            options.MatchEntireCellContents = false;
            options.CaseSensitive = false;

            // إنشاء إعداد الخط وعلم النمط
            string replacementText = "new text";
            FontSetting setting = new FontSetting(0, replacementText.Length, workbook.Worksheets);
            StyleFlag styleFlag = new StyleFlag();
            
            // تكوين الخط والنمط
            setting.Font.Color = Color.Red;
            setting.Font.Underline = FontUnderlineType.Single;
            styleFlag.FontColor = true;
            styleFlag.FontUnderline = true;

            // تطبيق الإعدادات على الخيارات
            options.FontSettings = new FontSetting[] { setting };
            options.StyleFlags = new StyleFlag[] { styleFlag };

            // تنفيذ الاستبدال
            workbook.Replace("test", replacementText, options);

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [StyleFlag](../../styleflag/)
* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


