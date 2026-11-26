---
title: "Comment.TextHorizontalAlignment"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Comment. Получает и задает тип горизонтального выравнивания текста комментария"
type: docs
url: /ru/net/aspose.cells/comment/texthorizontalalignment/
---
## Comment.TextHorizontalAlignment property

Получает и задает тип горизонтального выравнивания текста в комментарии.

```csharp
public TextAlignmentType TextHorizontalAlignment { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyTextHorizontalAlignmentDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить комментарий к ячейке A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Sample comment text";

            // Установить начальное горизонтальное выравнивание на Fill
            comment.TextHorizontalAlignment = TextAlignmentType.Fill;
            Console.WriteLine("Initial alignment: " + comment.TextHorizontalAlignment);

            // Изменить выравнивание на Center, если оно было Fill
            if (comment.TextHorizontalAlignment == TextAlignmentType.Fill)
            {
                comment.TextHorizontalAlignment = TextAlignmentType.Center;
                Console.WriteLine("Updated alignment: " + comment.TextHorizontalAlignment);
            }
        }
    }
}
```

### См. также

* enum [TextAlignmentType](../../textalignmenttype/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


