---
title: "RevisionCellComment.Row"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RevisionCellComment. Возвращает индекс строки, содержащей комментарий"
type: docs
url: /ru/net/aspose.cells.revisions/revisioncellcomment/row/
---
## RevisionCellComment.Row property

Получает индекс строки, в которой находится комментарий.

```csharp
public int Row { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellCommentPropertyRowDemo
    {
        public static void Run()
        {
            // Создать новую книгу с отслеживанием ревизий
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте комментарий в ячейку D4 (строка 3, столбец 3)
            int commentRow = 3;
            int commentCol = 3;
            Comment comment = worksheet.Comments[commentRow, commentCol];
            comment.Note = "Sample comment for revision tracking";

            // Изменить комментарий, чтобы создать ревизию
            comment.Note = "Updated comment text";

            // Получите доступ к ревизиям
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;
                    
                    // Отобразите значение свойства Row
                    Console.WriteLine("Comment is located at row: " + commentRevision.Row);
                    
                    // Продемонстрируйте использование свойства Row
                    Console.WriteLine("Comment location details:");
                    Console.WriteLine("Row index: " + commentRevision.Row);
                    Console.WriteLine("Column index: " + commentRevision.Column);
                    Console.WriteLine("Cell name: " + commentRevision.CellName);
                    
                    // Покажите, что Row только для чтения, попытавшись изменить его (это вызовет ошибку компиляции)
                    // commentRevision.Row = 5; // Эта строка закомментирована, так как Row только для чтения
                    
                    // Альтернативный способ изменить позицию, изменив CellName
                    Console.WriteLine("\nChanging comment position via CellName...");
                    commentRevision.CellName = "F10"; // Changes to row 9, column 5
                    Console.WriteLine("New Row index: " + commentRevision.Row);
                    Console.WriteLine("New Column index: " + commentRevision.Column);
                }
            }

            // Сохранить книгу с ревизиями
            workbook.Save("RevisionCellCommentPropertyRowDemo.xlsx");
        }
    }
}
```

### См. также

* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


