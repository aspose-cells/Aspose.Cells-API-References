---
title: "HtmlSaveOptions.DisableDownlevelRevealedComments"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlSaveOptions. تشير إلى ما إذا كان يتم تعطيل تعليقات Downlevelrevealed الشرطية عند تصدير الملف إلى html. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/disabledownlevelrevealedcomments/
---
## HtmlSaveOptions.DisableDownlevelRevealedComments property

يشير إلى ما إذا كان يتم تعطيل التعليقات الشرطية المكشوفة للمتصفحات القديمة عند تصدير الملف إلى html، القيمة الافتراضية هي false.

```csharp
public bool DisableDownlevelRevealedComments { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyDisableDownlevelRevealedCommentsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل تجريبي مع تعليق
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Comment comment = worksheet.Comments[worksheet.Comments.Add("A1")];
            comment.Note = "This is a test comment";

            // تعيين خيارات حفظ HTML مع DisableDownlevelRevealedComments
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.DisableDownlevelRevealedComments = true;

            // حفظ دفتر العمل مع خيارات HTML
            workbook.Save("output.html", options);
            
            Console.WriteLine("Workbook saved with DisableDownlevelRevealedComments=true");
        }
    }
}
```

### انظر أيضًا

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


