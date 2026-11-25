---
title: "Comment.HtmlNote"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Comment. Ottiene e imposta la stringa html che contiene dati e alcuni formati in questo commento"
type: docs
url: /it/net/aspose.cells/comment/htmlnote/
---
## Comment.HtmlNote property

Ottiene e imposta la stringa HTML che contiene dati e alcuni formati in questo commento.

```csharp
public string HtmlNote { get; set; }
```

### Osservazioni

Se questo è un commento a thread, la nota non può essere modificata, altrimenti MS Excel non potrebbe elaborarlo come commento a thread.

### Esempi

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

### Vedi anche

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


