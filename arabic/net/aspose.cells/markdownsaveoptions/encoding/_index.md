---
title: "MarkdownSaveOptions.Encoding"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية MarkdownSaveOptions. تحصل وتضبط الترميز الافتراضي"
type: docs
url: /ar/net/aspose.cells/markdownsaveoptions/encoding/
---
## MarkdownSaveOptions.Encoding property

يحصل على الترميز الافتراضي ويضبطه.

```csharp
public Encoding Encoding { get; set; }
```

### أمثلة

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MarkdownSaveOptionsPropertyEncodingDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Sample");
            worksheet.Cells["B1"].PutValue("Markdown");

            // قم بتكوين خيارات الحفظ باستخدام ترميز UTF8
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions
            {
                Encoding = Encoding.UTF8
            };

            // احفظ باستخدام الترميز المحدد
            workbook.Save("MarkdownWithEncoding.md", saveOptions);

            Console.WriteLine("Markdown file saved with UTF-8 encoding.");
        }
    }
}
```

### انظر أيضًا

* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


