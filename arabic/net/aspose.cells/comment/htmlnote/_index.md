---
title: "Comment.HtmlNote"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Comment. تحصل وتعيّن سلسلة html التي تحتوي على البيانات وبعض الصيغ في هذا التعليق"
type: docs
url: /ar/net/aspose.cells/comment/htmlnote/
---
## Comment.HtmlNote property

يحصل ويضبط سلسلة html التي تحتوي على البيانات وبعض التنسيقات في هذا التعليق.

```csharp
public string HtmlNote { get; set; }
```

### ملاحظات

إذا كان هذا تعليقًا متسلسلًا، لا يمكن تغيير الملاحظة، وإلا لن يتمكن MS Excel من معالجته كتعليق متسلسل.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyHtmlNoteDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            comment.HtmlNote = "<Font Style='FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;'>This is a <b>test</b>.</Font>";
            
            workbook.Save("CommentHtmlNoteDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


