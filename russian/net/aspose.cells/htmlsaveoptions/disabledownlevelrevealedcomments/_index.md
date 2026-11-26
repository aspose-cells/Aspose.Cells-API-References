---
title: "HtmlSaveOptions.DisableDownlevelRevealedComments"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Указывает, отключать ли условные комментарии Downlevelrevealed при экспорте файла в html; значение по умолчанию — false"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/disabledownlevelrevealedcomments/
---
## HtmlSaveOptions.DisableDownlevelRevealedComments property

Указывает, отключать ли условные комментарии Downlevel-revealed при экспорте файла в HTML, значение по умолчанию — false.

```csharp
public bool DisableDownlevelRevealedComments { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyDisableDownlevelRevealedCommentsDemo
    {
        public static void Run()
        {
            // Создать пример рабочей книги с комментарием
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Comment comment = worksheet.Comments[worksheet.Comments.Add("A1")];
            comment.Note = "This is a test comment";

            // Установить параметры сохранения HTML с DisableDownlevelRevealedComments
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.DisableDownlevelRevealedComments = true;

            // Сохранить рабочую книгу с параметрами HTML
            workbook.Save("output.html", options);
            
            Console.WriteLine("Workbook saved with DisableDownlevelRevealedComments=true");
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


