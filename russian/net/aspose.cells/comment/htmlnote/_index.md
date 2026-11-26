---
title: "Comment.HtmlNote"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Comment. Получает и задает html строку, содержащую данные и некоторые форматы в этом комментарии"
type: docs
url: /ru/net/aspose.cells/comment/htmlnote/
---
## Comment.HtmlNote property

Получает и задает HTML‑строку, содержащую данные и некоторые форматы в этом комментарии.

```csharp
public string HtmlNote { get; set; }
```

### Примечания

Если это threaded комментарий, заметку нельзя изменить, иначе MS Excel не сможет обработать его как threaded комментарий.

### Примеры

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

### См. также

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


