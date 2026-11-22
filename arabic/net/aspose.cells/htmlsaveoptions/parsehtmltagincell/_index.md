---
title: "HtmlSaveOptions.ParseHtmlTagInCell"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlSaveOptions. تشير إلى ما إذا كان يجب تحليل علامات HTML مثل div/div داخل الخلية كقيمة خلية أم الاحتفاظ بها كما هي. القيمة الافتراضية هي true"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/parsehtmltagincell/
---
## HtmlSaveOptions.ParseHtmlTagInCell property

يشير إلى ما إذا كان يجب تحليل علامة html (مثل `<div></div>`) في الخلية كقيمة خلية أو الحفاظ عليها كما هي. القيمة الافتراضية هي true.

```csharp
public bool ParseHtmlTagInCell { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyParseHtmlTagInCellDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل ببيانات تجريبية تحتوي على علامات HTML
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين قيمة الخلية مع علامات HTML
            worksheet.Cells["A1"].PutValue("<b>Bold Text</b> and <i>Italic Text</i>");
            
            // إنشاء خيارات حفظ HTML وتمكين تحليل علامات HTML
            HtmlSaveOptions htmlSaveOptions = new HtmlSaveOptions(SaveFormat.Html);
            htmlSaveOptions.ParseHtmlTagInCell = true;
            
            // حفظ دفتر العمل مع تحليل علامات HTML
            workbook.Save("output.html", htmlSaveOptions);
            
            Console.WriteLine("HTML saved with ParseHtmlTagInCell enabled.");
        }
    }
}
```

### انظر أيضًا

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


