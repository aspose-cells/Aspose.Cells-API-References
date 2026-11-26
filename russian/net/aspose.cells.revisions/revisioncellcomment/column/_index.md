---
title: "RevisionCellComment.Column"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RevisionCellComment. Возвращает индекс столбца, содержащего комментарий"
type: docs
url: /ru/net/aspose.cells.revisions/revisioncellcomment/column/
---
## RevisionCellComment.Column property

Получает индекс столбца, в котором находится комментарий.

```csharp
public int Column { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellCommentPropertyColumnDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте комментарий в ячейку D3
            int commentRow = 2;
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
                    
                    // Отобразите значение свойства Column
                    Console.WriteLine("Comment revision column index: " + commentRevision.Column);
                    
                    // Продемонстрируйте использование свойства Column
                    Console.WriteLine("Comment was modified in column: " + (char)('A' + commentRevision.Column));
                    
                    // Показать связанные свойства
                    Console.WriteLine("Associated row: " + commentRevision.Row);
                    Console.WriteLine("Cell name: " + commentRevision.CellName);
                    
                    // Примечание: свойство Column только для чтения, поэтому его нельзя изменить напрямую
                    // Мы можем изменить его косвенно, изменив CellName
                    string originalCellName = commentRevision.CellName;
                    commentRevision.CellName = "E5"; // This will update both Row and Column properties
                    Console.WriteLine("After CellName change - New column: " + commentRevision.Column);
                    
                    // Восстановить исходное значение
                    commentRevision.CellName = originalCellName;
                }
            }

            // Сохранить книгу с ревизиями
            workbook.Save("RevisionCellCommentPropertyColumnDemo.xlsx");
        }
    }
}
```

### См. также

* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


