---
title: "Comment.HtmlNote"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Comment-Eigenschaft. Ruft die HTML-Zeichenfolge ab, die Daten und einige Formate in diesem Kommentar enthält, und legt sie fest"
type: docs
url: /de/net/aspose.cells/comment/htmlnote/
---
## Comment.HtmlNote property

Liest und setzt die HTML-Zeichenkette, die Daten und einige Formate in diesem Kommentar enthält.

```csharp
public string HtmlNote { get; set; }
```

### Hinweise

Wenn dies ein Threaded‑Kommentar ist, kann die Notiz nicht geändert werden, sonst könnte MS Excel ihn nicht als Threaded‑Kommentar verarbeiten.

### Beispiele

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

### Siehe auch

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


