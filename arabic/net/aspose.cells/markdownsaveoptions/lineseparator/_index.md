---
title: "MarkdownSaveOptions.LineSeparator"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية MarkdownSaveOptions. تحصل وتضبط فاصل السطر"
type: docs
url: /ar/net/aspose.cells/markdownsaveoptions/lineseparator/
---
## MarkdownSaveOptions.LineSeparator property

يحصل على فاصل السطر ويضبطه.

```csharp
public string LineSeparator { get; set; }
```

### أمثلة

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MarkdownSaveOptionsPropertyLineSeparatorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Value1");
            worksheet.Cells["B2"].PutValue("Value2");

            // قم بتكوين خيارات حفظ Markdown باستخدام فاصل سطر مخصص
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions
            {
                LineSeparator = "\n", // Using Unix-style line endings
                Encoding = Encoding.UTF8
            };

            // حفظ كملف Markdown
            workbook.Save("MarkdownWithLineSeparator.md", saveOptions);

            Console.WriteLine("Markdown file saved with custom line separator.");
        }
    }
}
```

### انظر أيضًا

* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


