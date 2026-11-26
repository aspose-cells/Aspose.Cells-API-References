---
title: "Перечисление PrintCommentsType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.PrintCommentsType. Представляет способ печати комментариев на листе"
type: docs
url: /ru/net/aspose.cells/printcommentstype/
---
## PrintCommentsType enumeration

Представляет способ печати комментариев вместе с листом.

```csharp
public enum PrintCommentsType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| PrintInPlace | `0` | Представляет печать комментариев в виде, отображаемом на листе. |
| PrintNoComments | `1` | Представляет отсутствие печати комментариев. |
| PrintSheetEnd | `2` | Представляет печать комментариев в конце листа. |
| PrintWithThreadedComments | `3` | Представляет печать комментариев в виде, отображаемом на листе, включая ветвящиеся комментарии. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PrintCommentsTypeDemo
    {
        public static void PrintCommentsTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте несколько комментариев в лист
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a comment.";

            commentIndex = worksheet.Comments.Add("B2");
            comment = worksheet.Comments[commentIndex];
            comment.Note = "This is another comment.";

            // Установите тип печати комментариев в настройках страницы
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.PrintComments = PrintCommentsType.PrintSheetEnd;

            // Сохранить книгу в файл
            workbook.Save("PrintCommentsTypeExample.xlsx");

            Console.WriteLine("Workbook saved successfully with comments printed at the end of the sheet.");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


