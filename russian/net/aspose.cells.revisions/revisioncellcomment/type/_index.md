---
title: "RevisionCellComment.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RevisionCellComment. Возвращает тип правки"
type: docs
url: /ru/net/aspose.cells.revisions/revisioncellcomment/type/
---
## RevisionCellComment.Type property

Получает тип ревизии.

```csharp
public override RevisionType Type { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellCommentPropertyTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить комментарий к ячейке A1
            int commentRow = 0;
            int commentCol = 0;
            Comment comment = worksheet.Comments[commentRow, commentCol];
            comment.Note = "Initial comment";

            // Отслеживание правок — изменено для использования свойства HasRevisions
            // Примечание: В реальном использовании вам может потребоваться включить отслеживание другими способами
            // поскольку HasRevisions является свойством только для чтения, которое указывает, существуют ли правки

            // Изменить комментарий, чтобы создать ревизию
            comment.Note = "Modified comment";

            // Получите доступ к правкам через коллекцию RevisionLogs книги Workbook
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;
                    
                    // Отобразите значение свойства Type
                    Console.WriteLine("Revision Type: " + commentRevision.Type);
                    
                    // Продемонстрировать использование свойства Type
                    if (commentRevision.Type == RevisionType.Comment)
                    {
                        Console.WriteLine("This revision is related to a comment change");
                        Console.WriteLine("Comment was modified at row: " + commentRevision.Row + ", column: " + commentRevision.Column);
                        Console.WriteLine("Old comment length: " + commentRevision.OldLength);
                        Console.WriteLine("New comment length: " + commentRevision.NewLength);
                    }
                }
            }

            // Сохранить книгу с ревизиями
            workbook.Save("RevisionCellCommentPropertyTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [RevisionType](../../revisiontype/)
* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


