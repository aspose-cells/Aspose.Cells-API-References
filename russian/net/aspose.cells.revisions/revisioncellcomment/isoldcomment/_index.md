---
title: "RevisionCellComment.IsOldComment"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RevisionCellComment. Указывает, является ли комментарий старым"
type: docs
url: /ru/net/aspose.cells.revisions/revisioncellcomment/isoldcomment/
---
## RevisionCellComment.IsOldComment property

Указывает, является ли комментарий старым.

```csharp
public bool IsOldComment { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellCommentPropertyIsOldCommentDemo
    {
        public static void Run()
        {
            // Создать новую книгу с отслеживанием ревизий
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить начальный комментарий в ячейку A1
            Comment comment = worksheet.Comments[0, 0];
            comment.Note = "First version of comment";

            // Изменить комментарий, чтобы создать ревизию
            comment.Note = "Updated comment text";

            // Добавьте ещё один комментарий в ячейку B2
            Comment secondComment = worksheet.Comments[1, 1];
            secondComment.Note = "Second comment";

            // Получите доступ к ревизиям
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;
                    
                    // Отобразите значение свойства IsOldComment
                    Console.WriteLine("Cell: " + commentRevision.CellName);
                    Console.WriteLine("IsOldComment: " + commentRevision.IsOldComment);
                    
                    // Продемонстрируйте использование свойства IsOldComment
                    if (commentRevision.IsOldComment)
                    {
                        Console.WriteLine("This revision represents the old state of the comment");
                        Console.WriteLine("Old comment length: " + commentRevision.OldLength);
                    }
                    else
                    {
                        Console.WriteLine("This revision represents the new state of the comment");
                        Console.WriteLine("New comment length: " + commentRevision.NewLength);
                    }

                    // Показать связанные свойства
                    Console.WriteLine("Action Type: " + commentRevision.ActionType);
                    Console.WriteLine("Revision Type: " + commentRevision.Type);
                }
            }

            // Сохранить книгу с ревизиями
            workbook.Save("RevisionCellCommentPropertyIsOldCommentDemo.xlsx");
        }
    }
}
```

### См. также

* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


