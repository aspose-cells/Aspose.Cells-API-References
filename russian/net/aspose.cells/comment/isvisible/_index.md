---
title: "Comment.IsVisible"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Comment. Представляет, видим ли комментарий или нет"
type: docs
url: /ru/net/aspose.cells/comment/isvisible/
---
## Comment.IsVisible property

Указывает, видим ли комментарий.

```csharp
public bool IsVisible { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить комментарий к ячейке A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a test comment";

            // Установить комментарий видимым
            comment.IsVisible = true;

            // Проверить, видим ли комментарий
            if (comment.IsVisible)
            {
                Console.WriteLine("The comment is visible");
            }

            // Сохраните книгу
            workbook.Save("CommentVisibilityDemo.xlsx");
        }
    }
}
```

### См. также

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


