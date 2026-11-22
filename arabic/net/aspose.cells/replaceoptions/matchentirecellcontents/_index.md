---
title: "ReplaceOptions.MatchEntireCellContents"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ReplaceOptions. تشير إلى ما إذا كان يجب مطابقة محتويات الخلايا بالكامل"
type: docs
url: /ar/net/aspose.cells/replaceoptions/matchentirecellcontents/
---
## ReplaceOptions.MatchEntireCellContents property

يشير إلى ما إذا كان يجب مطابقة محتويات الخلايا بالكامل

```csharp
public bool MatchEntireCellContents { get; set; }
```

### ملاحظات

القيمة الافتراضية هي true.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReplaceOptionsPropertyMatchEntireCellContentsDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين قيم خلايا العينة
            worksheet.Cells["A1"].PutValue("apple");
            worksheet.Cells["A2"].PutValue("apple pie");
            worksheet.Cells["A3"].PutValue("an apple");
            worksheet.Cells["A4"].PutValue("apples");

            // استبدال مع MatchEntireCellContents = true (مطابقة دقيقة فقط)
            ReplaceOptions options1 = new ReplaceOptions();
            options1.MatchEntireCellContents = true;
            workbook.Replace("apple", "orange", options1);

            // استبدال مع MatchEntireCellContents = false (مطابقة جزئية)
            ReplaceOptions options2 = new ReplaceOptions();
            options2.MatchEntireCellContents = false;
            workbook.Replace("apple", "banana", options2);

            // إخراج النتائج
            Console.WriteLine("A1: " + worksheet.Cells["A1"].StringValue); // orange (exact match)
            Console.WriteLine("A2: " + worksheet.Cells["A2"].StringValue); // banana pie (partial match)
            Console.WriteLine("A3: " + worksheet.Cells["A3"].StringValue); // an banana (partial match)
            Console.WriteLine("A4: " + worksheet.Cells["A4"].StringValue); // bananas (partial match)
        }
    }
}
```

### انظر أيضًا

* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


