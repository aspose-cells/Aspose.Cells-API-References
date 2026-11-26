---
title: "RevisionCellComment.NewLength"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RevisionCellComment. Возвращает длину комментария до внесения этой правки"
type: docs
url: /ru/net/aspose.cells.revisions/revisioncellcomment/newlength/
---
## RevisionCellComment.NewLength property

Получает длину комментария до внесения этой ревизии.

```csharp
public int NewLength { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellCommentPropertyNewLengthDemo
    {
        public static void Run()
        {
            // Создать новую книгу с отслеживанием ревизий
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте комментарий в ячейку F7
            int commentRow = 6;
            int commentCol = 5;
            Comment comment = worksheet.Comments[commentRow, commentCol];
            comment.Note = "Initial comment text";

            // Изменить комментарий, чтобы создать ревизию
            string updatedComment = "This is an updated and longer comment text";
            comment.Note = updatedComment;

            // Получите доступ к ревизиям
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;
                    
                    // Отобразите значение свойства NewLength
                    Console.WriteLine("New comment length: " + commentRevision.NewLength);
                    Console.WriteLine("Actual new comment length: " + updatedComment.Length);
                    
                    // Отобразите связанные свойства
                    Console.WriteLine("Old comment length: " + commentRevision.OldLength);
                    Console.WriteLine("Comment location: " + commentRevision.CellName);
                    
                    // Продемонстрируйте использование свойства NewLength
                    if (commentRevision.NewLength > commentRevision.OldLength)
                    {
                        Console.WriteLine("Comment was expanded by " + 
                            (commentRevision.NewLength - commentRevision.OldLength) + " characters");
                    }
                    else if (commentRevision.NewLength < commentRevision.OldLength)
                    {
                        Console.WriteLine("Comment was shortened by " + 
                            (commentRevision.OldLength - commentRevision.NewLength) + " characters");
                    }
                    else
                    {
                        Console.WriteLine("Comment length remained the same");
                    }
                }
            }

            // Сохранить книгу с ревизиями
            workbook.Save("RevisionCellCommentPropertyNewLengthDemo.xlsx");
        }
    }
}
```

### См. также

* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


