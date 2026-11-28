---
title: "Comment.HtmlNote"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Comment özelliği. Bu yorumda veri ve bazı biçimleri içeren html dizesini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/comment/htmlnote/
---
## Comment.HtmlNote property

Bu yorumda veri ve bazı biçimleri içeren html dizesini alır ve ayarlar.

```csharp
public string HtmlNote { get; set; }
```

### Açıklamalar

Bu bir zincirleme yorum ise, not değiştirilemez, aksi takdirde MS Excel bunu zincirleme yorum olarak işleyemez.

### Örnekler

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

### Ayrıca Bakınız

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


