---
title: "Comment.Note"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Comment. Представляет содержимое комментария"
type: docs
url: /ru/net/aspose.cells/comment/note/
---
## Comment.Note property

Представляет содержание комментария.

```csharp
public string Note { get; set; }
```

### Примечания

Если это threaded комментарий, заметку нельзя изменить, иначе MS Excel не сможет обработать его как threaded комментарий.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyNoteDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить комментарий к ячейке A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment1 = worksheet.Comments[commentIndex];
            
            // Установить примечание для комментария
            comment1.Note = "First note.";
            
            // Проверьте, что примечание было установлено
            Console.WriteLine("Comment note: " + comment1.Note);
        }
    }
}
```

### См. также

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


