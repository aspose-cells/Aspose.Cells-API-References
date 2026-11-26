---
title: "Comment.AutoSize"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Comment. Указывает, автоматически ли размер комментария регулируется в соответствии с его содержимым. Примечание: в некоторых особых случаях, например в среде Mac, эта настройка может не срабатывать. Если настройка не срабатывает, пожалуйста, замените её на FitToTextSize"
type: docs
url: /ru/net/aspose.cells/comment/autosize/
---
## Comment.AutoSize property

Указывает, автоматически ли размер комментария регулируется в соответствии с его содержимым. Примечание: в некоторых особых случаях (например, в среде Mac) эта настройка может не сработать. Если настройка не сработает, замените её вызовом FitToTextSize().

```csharp
public bool AutoSize { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyAutoSizeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить комментарий к ячейке A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a sample comment that will auto-size to fit its content.";

            // Установить AutoSize в true
            comment.AutoSize = true;

            // Сохраните книгу
            workbook.Save("CommentAutoSizeDemo.xlsx");
        }
    }
}
```

### См. также

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


