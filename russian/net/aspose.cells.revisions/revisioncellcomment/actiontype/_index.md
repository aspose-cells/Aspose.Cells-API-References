---
title: "RevisionCellComment.ActionType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RevisionCellComment. Возвращает тип действия правки"
type: docs
url: /ru/net/aspose.cells.revisions/revisioncellcomment/actiontype/
---
## RevisionCellComment.ActionType property

Получает тип действия ревизии.

```csharp
public RevisionActionType ActionType { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellCommentPropertyActionTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу с отслеживанием ревизий
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить комментарий к ячейке A1
            Comment comment = worksheet.Comments[0, 0];
            comment.Note = "Initial comment";

            // Изменить комментарий, чтобы создать ревизию
            comment.Note = "Updated comment";

            // Добавьте новый комментарий, чтобы сгенерировать правку Add
            Comment newComment = worksheet.Comments[1, 1];
            newComment.Note = "New comment";

            // Получите доступ к ревизиям
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;
                    
                    // Отобразите значение свойства ActionType
                    Console.WriteLine("Revision ActionType: " + commentRevision.ActionType);
                    
                    // Продемонстрировать использование свойства ActionType
                    switch (commentRevision.ActionType)
                    {
                        case RevisionActionType.Add:
                            Console.WriteLine("This revision added a new comment at " + commentRevision.CellName);
                            break;
                        case RevisionActionType.Delete:
                            Console.WriteLine("This revision deleted a comment from " + commentRevision.CellName);
                            break;
                        default:
                            Console.WriteLine("This revision modified a comment at " + commentRevision.CellName);
                            break;
                    }

                    // Показать связанные свойства
                    Console.WriteLine("Comment location: " + commentRevision.CellName);
                    Console.WriteLine("Is old comment: " + commentRevision.IsOldComment);
                    Console.WriteLine("Old length: " + commentRevision.OldLength);
                    Console.WriteLine("New length: " + commentRevision.NewLength);
                }
            }

            // Сохранить книгу с ревизиями
            workbook.Save("RevisionCellCommentPropertyActionTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [RevisionActionType](../../revisionactiontype/)
* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


