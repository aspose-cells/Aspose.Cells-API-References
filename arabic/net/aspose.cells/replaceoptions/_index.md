---
title: "الفئة ReplaceOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.ReplaceOptions. تمثيل خيارات الاستبدال"
type: docs
url: /ar/net/aspose.cells/replaceoptions/
---
## ReplaceOptions class

يمثل خيارات الاستبدال.

```csharp
public class ReplaceOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [ReplaceOptions](replaceoptions/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CaseSensitive](../../aspose.cells/replaceoptions/casesensitive/) { get; set; } | يشير إلى ما إذا كانت السلسلة التي تم البحث عنها حساسة لحالة الأحرف. |
| [FontSettings](../../aspose.cells/replaceoptions/fontsettings/) { get; set; } | إعدادات التنسيق الغني للنص المستبدل. |
| [MatchEntireCellContents](../../aspose.cells/replaceoptions/matchentirecellcontents/) { get; set; } | يشير إلى ما إذا كان يجب مطابقة محتويات الخلايا بالكامل |
| [RegexKey](../../aspose.cells/replaceoptions/regexkey/) { get; set; } | يشير إلى ما إذا كان المفتاح المُبحث هو تعبير نمطي. إذا كان صحيحًا فسيُعامل المفتاح المُبحث كتعبير نمطي. |
| [StyleFlags](../../aspose.cells/replaceoptions/styleflags/) { get; set; } | يحصل على ويضبط علامات تطبيق إعدادات الخط. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ReplaceOptionsDemo
    {
        public static void ReplaceOptionsExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة بعض البيانات النموذجية إلى ورقة العمل
            sheet.Cells["A1"].PutValue("Hello World");
            sheet.Cells["A2"].PutValue("Hello Aspose");
            sheet.Cells["A3"].PutValue("Goodbye World");

            // إنشاء ReplaceOptions
            ReplaceOptions options = new ReplaceOptions
            {
                CaseSensitive = false,
                MatchEntireCellContents = false,
                RegexKey = false
            };

            // استبدال "Hello" بـ "Hi" في ورقة العمل
            int replacedCount = workbook.Replace("Hello", "Hi", options);

            // إخراج عدد الاستبدالات التي تم إجراؤها
            Console.WriteLine($"Number of replacements made: {replacedCount}");

            // احفظ المصنف
            workbook.Save("ReplaceOptionsExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


