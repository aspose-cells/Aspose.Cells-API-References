---
title: "HtmlSaveOptions.ExportWorkbookProperties"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Указывает, экспортировать ли свойства рабочей книги. Значение по умолчанию — true. Если вы хотите импортировать html или mht файл в Excel, оставьте значение по умолчанию."
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/exportworkbookproperties/
---
## HtmlSaveOptions.ExportWorkbookProperties property

Указывает, экспортировать ли свойства рабочей книги.Значение по умолчанию — true.If вы хотите импортировать файл html или mht в Excel, пожалуйста, оставьте значение по умолчанию.

```csharp
public bool ExportWorkbookProperties { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportWorkbookPropertiesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавьте некоторые данные в рабочую книгу
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // Установите свойства рабочей книги
            workbook.BuiltInDocumentProperties.Author = "Test Author";
            workbook.BuiltInDocumentProperties.Title = "Test Title";

            // Создать параметры сохранения HTML
            HtmlSaveOptions options = new HtmlSaveOptions();
            
            // Продемонстрируйте ExportWorkbookProperties, установив его в false
            options.ExportWorkbookProperties = false;
            
            // Сохраните книгу в формате HTML
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML file saved with ExportWorkbookProperties set to false");
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


