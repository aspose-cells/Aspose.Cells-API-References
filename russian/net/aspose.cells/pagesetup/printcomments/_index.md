---
title: "PageSetup.PrintComments"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PageSetup. Представляет способ печати комментариев вместе с листом"
type: docs
url: /ru/net/aspose.cells/pagesetup/printcomments/
---
## PageSetup.PrintComments property

Представляет способ печати комментариев вместе с листом.

```csharp
public PrintCommentsType PrintComments { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintCommentsDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить комментарий к ячейке A1
            int commentIndex = sheet.Comments.Add("A1");
            Comment comment = sheet.Comments[commentIndex];
            comment.Note = "This is a test comment";

            // Установите различные параметры печати комментариев и продемонстрируйте их эффекты
            sheet.PageSetup.PrintComments = PrintCommentsType.PrintInPlace;
            Console.WriteLine("PrintComments set to PrintInPlace");

            sheet.PageSetup.PrintComments = PrintCommentsType.PrintSheetEnd;
            Console.WriteLine("PrintComments set to PrintSheetEnd");

            sheet.PageSetup.PrintComments = PrintCommentsType.PrintNoComments;
            Console.WriteLine("PrintComments set to PrintNoComments");

            // Сохраните книгу, чтобы продемонстрировать сохранность настроек
            workbook.Save("PrintCommentsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* enum [PrintCommentsType](../../printcommentstype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


