---
title: "TxtSaveOptions.ExportQuotePrefix"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TxtSaveOptions. تشير إلى ما إذا كان يجب تصدير علامة الاقتباس المفردة كجزء من قيمة خلية واحدة عندما تكون QuotePrefix مفعلة لها. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/txtsaveoptions/exportquoteprefix/
---
## TxtSaveOptions.ExportQuotePrefix property

تشير إلى ما إذا كان يجب تصدير علامة الاقتباس المفردة كجزء من قيمة خلية واحدة عندما تكون [`QuotePrefix`](../../style/quoteprefix/) مفعلة لها. القيمة الافتراضية هي false.

```csharp
public bool ExportQuotePrefix { get; set; }
```

### أمثلة

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyExportQuotePrefixDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // إضافة بيانات نموذجية مع أحرف خاصة
            cells[0, 0].PutValue("a\\bcdef\"g");
            cells[0, 1].PutValue("f\"g");
            cells[0, 2].PutValue("a\\bcdg");
            cells[0, 3].PutValue("abcdefg");
            cells[0, 4].PutValue("efg");
            cells[0, 5].PutValue("'abc");

            // إنشاء خيارات حفظ TXT
            TxtSaveOptions saveOptions = new TxtSaveOptions
            {
                Encoding = Encoding.ASCII,
                Separator = ',',
                ExportQuotePrefix = true // Demonstrate ExportQuotePrefix property
            };

            // حفظ مع ExportQuotePrefix = true
            workbook.Save("output_with_exportquoteprefix.csv", saveOptions);

            // تغيير الفاصل وحفظ مرة أخرى
            saveOptions.Separator = '\\';
            workbook.Save("output_with_backslash_separator.csv", saveOptions);

            Console.WriteLine("Files saved successfully with ExportQuotePrefix property.");
        }
    }
}
```

### انظر أيضًا

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


