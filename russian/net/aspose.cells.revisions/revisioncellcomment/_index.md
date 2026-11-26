---
title: "Класс RevisionCellComment"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Revisions.RevisionCellComment. Представляет запись ревизии изменения комментария ячейки"
type: docs
url: /ru/net/aspose.cells.revisions/revisioncellcomment/
---
## RevisionCellComment class

Представляет запись ревизии изменения комментария ячейки.

```csharp
public class RevisionCellComment : Revision
```

## Свойства

| Имя | Описание |
| --- | --- |
| [ActionType](../../aspose.cells.revisions/revisioncellcomment/actiontype/) { get; } | Получает тип действия ревизии. |
| [CellName](../../aspose.cells.revisions/revisioncellcomment/cellname/) { get; set; } | Получает имя ячейки. |
| [Column](../../aspose.cells.revisions/revisioncellcomment/column/) { get; } | Получает индекс столбца, в котором находится комментарий. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Получает номер этой ревизии.(Наследовано от [`Revision`](../revision/).) |
| [IsOldComment](../../aspose.cells.revisions/revisioncellcomment/isoldcomment/) { get; } | Указывает, является ли комментарий старым. |
| [NewLength](../../aspose.cells.revisions/revisioncellcomment/newlength/) { get; } | Получает длину комментария до внесения этой ревизии. |
| [OldLength](../../aspose.cells.revisions/revisioncellcomment/oldlength/) { get; } | Получает длину текста комментария, добавленного в этой ревизии. |
| [Row](../../aspose.cells.revisions/revisioncellcomment/row/) { get; } | Получает индекс строки, в которой находится комментарий. |
| override [Type](../../aspose.cells.revisions/revisioncellcomment/type/) { get; } | Получает тип ревизии. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Получает лист.(Наследовано от [`Revision`](../revision/).) |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionCellCommentDemo
    {
        public static void Run()
        {
            // Создать новую книгу с отслеживанием ревизий
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить начальный комментарий в ячейку A1
            Comment comment = worksheet.Comments[0, 0];
            comment.Note = "Initial comment text";

            // Изменить комментарий, чтобы создать ревизию
            comment.Note = "Updated comment with more text";

            // Получить доступ к журналу ревизий
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;

                    // Отобразить свойства ревизии
                    Console.WriteLine("Revision Type: " + commentRevision.Type);
                    Console.WriteLine("Action Type: " + commentRevision.ActionType);
                    Console.WriteLine("Cell Location: " + commentRevision.CellName);
                    Console.WriteLine("Row: " + commentRevision.Row);
                    Console.WriteLine("Column: " + commentRevision.Column);

                    // Показать изменения длины комментария
                    Console.WriteLine("Old Length: " + commentRevision.OldLength);
                    Console.WriteLine("New Length: " + commentRevision.NewLength);
                    Console.WriteLine("Is Old Comment: " + commentRevision.IsOldComment);

                    // Изменить имя ячейки, чтобы продемонстрировать изменение свойства
                    string originalCellName = commentRevision.CellName;
                    commentRevision.CellName = "B2";
                    Console.WriteLine("Modified Cell Location: " + commentRevision.CellName);
                    Console.WriteLine("New Row: " + commentRevision.Row);
                    Console.WriteLine("New Column: " + commentRevision.Column);

                    // Восстановить оригинальное имя ячейки
                    commentRevision.CellName = originalCellName;
                }
            }

            // Сохранить книгу с ревизиями
            workbook.Save("RevisionsClassRevisionCellCommentDemo.xlsx");
        }
    }
}
```

### См. также

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


