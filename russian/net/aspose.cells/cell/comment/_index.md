---
title: "Cell.Comment"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cell. Получает комментарий этой ячейки"
type: docs
url: /ru/net/aspose.cells/cell/comment/
---
## Cell.Comment property

Получает комментарий этой ячейки.

```csharp
public Comment Comment { get; }
```

### Примечания

Если к ячейке не применён комментарий, возвращает null.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellPropertyCommentDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить комментарий к ячейке A1
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Cell");

            // Добавить комментарий к ячейке
            Comment comment = cell.Comment;
            if (comment == null)
            {
                // Создать новый комментарий, если он отсутствует
                int commentIndex = worksheet.Comments.Add("A1");
                comment = worksheet.Comments[commentIndex];
                comment.Author = "Author Name";
                comment.Note = "This is a sample comment";
            }

            try
            {
                // Отобразить свойства комментария
                Console.WriteLine("Comment Author: " + comment.Author);
                Console.WriteLine("Comment Note: " + comment.Note);
                Console.WriteLine("Comment Row: " + comment.Row);
                Console.WriteLine("Comment Column: " + comment.Column);
                Console.WriteLine("Comment is Visible: " + comment.IsVisible);

                // Изменить некоторые свойства комментария
                comment.Note = "Updated comment text";
                comment.IsVisible = true;

                // Отобразить обновлённую заметку комментария
                Console.WriteLine("Updated Comment Note: " + comment.Note);

                // Сохраните книгу
                workbook.Save("CommentDemo.xlsx");
                Console.WriteLine("Comment has been demonstrated and saved to CommentDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [Comment](../../comment/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


