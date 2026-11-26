---
title: "HtmlSaveOptions.IsExportComments"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Указывает, экспортировать ли комментарии при сохранении файла в HTML. Значение по умолчанию — false"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/isexportcomments/
---
## HtmlSaveOptions.IsExportComments property

Указывает, экспортировать ли комментарии при сохранении файла в HTML, значение по умолчанию — false.

```csharp
public bool IsExportComments { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIsExportCommentsDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными и комментариями
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // Добавить комментарий
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a test comment";
            
            // Сохраните с IsExportComments = false (комментарии не будут экспортированы)
            HtmlSaveOptions options1 = new HtmlSaveOptions
            {
                IsExportComments = false
            };
            workbook.Save("output_without_comments.html", options1);
            
            // Сохраните с IsExportComments = true (комментарии будут экспортированы)
            HtmlSaveOptions options2 = new HtmlSaveOptions
            {
                IsExportComments = true
            };
            workbook.Save("output_with_comments.html", options2);
            
            Console.WriteLine("HTML files created successfully.");
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


