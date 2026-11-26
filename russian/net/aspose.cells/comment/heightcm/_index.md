---
title: "Comment.HeightCM"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Comment. Представляет высоту комментария в сантиметрах"
type: docs
url: /ru/net/aspose.cells/comment/heightcm/
---
## Comment.HeightCM property

Представляет высоту комментария в сантиметрах.

```csharp
public double HeightCM { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyHeightCMDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить комментарий к ячейке A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            // Установить текст комментария
            comment.Note = "Sample comment";
            
            // Установить высоту комментария в сантиметрах
            comment.HeightCM = 1.5;
            
            // Сохраните книгу
            workbook.Save("CommentHeightCMDemo.xlsx");
        }
    }
}
```

### См. также

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


