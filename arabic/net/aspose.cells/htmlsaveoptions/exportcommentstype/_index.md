---
title: "HtmlSaveOptions.ExportCommentsType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlSaveOptions. تمثل نوع تصدير التعليقات إلى ملفات html"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/exportcommentstype/
---
## HtmlSaveOptions.ExportCommentsType property

يمثل نوع تصدير التعليقات إلى ملفات html.

```csharp
public PrintCommentsType ExportCommentsType { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportCommentsTypeDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة تعليق تجريبي باستخدام اسم الخلية
            Comment comment = worksheet.Comments["A1"];
            comment.Note = "This is a test comment";
            
            // تعيين خيارات حفظ HTML باستخدام ExportCommentsType
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportCommentsType = PrintCommentsType.PrintInPlace;
            
            // حفظ إلى HTML
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("HTML file with comments exported successfully.");
        }
    }
}
```

### انظر أيضًا

* enum [PrintCommentsType](../../printcommentstype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


