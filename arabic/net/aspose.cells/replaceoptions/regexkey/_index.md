---
title: "ReplaceOptions.RegexKey"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ReplaceOptions. تشير إلى ما إذا كان المفتاح الذي تم البحث عنه regex. إذا كان true فسيتم اعتبار المفتاح الذي تم البحث عنه ك regex"
type: docs
url: /ar/net/aspose.cells/replaceoptions/regexkey/
---
## ReplaceOptions.RegexKey property

يشير إلى ما إذا كان المفتاح المُبحث هو تعبير نمطي. إذا كان صحيحًا فسيُعامل المفتاح المُبحث كتعبير نمطي.

```csharp
public bool RegexKey { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReplaceOptionsPropertyRegexKeyDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل مع بيانات عينة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("apple");
            worksheet.Cells["A2"].PutValue("banana");
            worksheet.Cells["A3"].PutValue("orange");
            worksheet.Cells["A4"].PutValue("pear");
            worksheet.Cells["A5"].PutValue("plum");

            // إنشاء خيارات الاستبدال مع regex
            ReplaceOptions options = new ReplaceOptions();
            options.RegexKey = true; // Enable regex matching
            
            // استبدال جميع الكلمات التي تبدأ بـ 'p' أو 'b' وتليها حرف علة
            string pattern = "^[pb][aeiou]";
            string replacement = "FRUIT";
            
            // تنفيذ الاستبدال
            workbook.Replace(pattern, replacement, options);

            // حفظ النتيجة
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


