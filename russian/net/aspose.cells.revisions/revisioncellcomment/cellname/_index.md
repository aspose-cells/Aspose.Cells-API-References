---
title: "RevisionCellComment.CellName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RevisionCellComment. Возвращает имя ячейки"
type: docs
url: /ru/net/aspose.cells.revisions/revisioncellcomment/cellname/
---
## RevisionCellComment.CellName property

Получает имя ячейки.

```csharp
public string CellName { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellCommentPropertyCellNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте комментарий в ячейку B5
            int commentRow = 4;
            int commentCol = 1;
            Comment comment = worksheet.Comments[commentRow, commentCol];
            comment.Note = "Initial comment";

            // Изменить комментарий, чтобы создать ревизию
            comment.Note = "Updated comment";

            // Получите доступ к ревизиям
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;
                    
                    // Отобразите текущее значение CellName
                    Console.WriteLine("Original CellName: " + commentRevision.CellName);
                    
                    // Измените свойство CellName
                    commentRevision.CellName = "C10";
                    Console.WriteLine("Modified CellName: " + commentRevision.CellName);
                    
                    // Продемонстрируйте эффект изменения CellName
                    Console.WriteLine("Row index: " + commentRevision.Row);
                    Console.WriteLine("Column index: " + commentRevision.Column);
                    
                    // Примечание: изменение CellName обновляет свойства Row/Column
                    Console.WriteLine("After CellName change - Row: " + commentRevision.Row);
                    Console.WriteLine("After CellName change - Column: " + commentRevision.Column);
                }
            }

            // Сохранить книгу с ревизиями
            workbook.Save("RevisionCellCommentPropertyCellNameDemo.xlsx");
        }
    }
}
```

### См. также

* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


