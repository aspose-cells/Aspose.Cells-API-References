---
title: "Comment.TextVerticalAlignment"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Comment. Получает и задает тип вертикального выравнивания текста комментария"
type: docs
url: /ru/net/aspose.cells/comment/textverticalalignment/
---
## Comment.TextVerticalAlignment property

Получает и задает тип вертикального выравнивания текста в комментарии.

```csharp
public TextAlignmentType TextVerticalAlignment { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyTextVerticalAlignmentDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int commentIndex = worksheet.Comments.Add("B3");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Sample comment text";

            // Установить вертикальное выравнивание на Fill
            comment.TextVerticalAlignment = TextAlignmentType.Fill;
            Console.WriteLine("Vertical Alignment: " + comment.TextVerticalAlignment);

            // Изменить вертикальное выравнивание на Center, если оно было Fill
            if (comment.TextVerticalAlignment == TextAlignmentType.Fill)
            {
                comment.TextVerticalAlignment = TextAlignmentType.Center;
                Console.WriteLine("Changed Vertical Alignment to: " + comment.TextVerticalAlignment);
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


