---
title: "Comment.HtmlNote"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Comment-egenskap. Hämtar och anger html-strängen som innehåller data och vissa format i denna kommentar"
type: docs
url: /sv/net/aspose.cells/comment/htmlnote/
---
## Comment.HtmlNote property

Hämtar och anger html-strängen som innehåller data och vissa format i denna kommentar.

```csharp
public string HtmlNote { get; set; }
```

### Anmärkningar

Om detta är en trådad kommentar kan noteringen inte ändras, annars kan MS Excel inte behandla den som en trådad kommentar.

### Exempel

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

### Se även

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


