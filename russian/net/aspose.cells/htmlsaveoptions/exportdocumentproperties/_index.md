---
title: "HtmlSaveOptions.ExportDocumentProperties"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Указывает, экспортировать ли свойства документа. Значение по умолчанию — true. Если вы хотите импортировать файл html или mht в Excel, пожалуйста, оставьте значение по умолчанию"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/exportdocumentproperties/
---
## HtmlSaveOptions.ExportDocumentProperties property

Указывает, экспортировать ли свойства документа.Значение по умолчанию — true.If вы хотите импортировать файл html или mht в Excel, пожалуйста, оставьте значение по умолчанию.

```csharp
public bool ExportDocumentProperties { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportDocumentPropertiesDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте некоторые свойства документа
            workbook.BuiltInDocumentProperties.Author = "Test Author";
            workbook.BuiltInDocumentProperties.Title = "Test Document";
            
            // Добавьте примерные данные ячеек
            worksheet.Cells["A1"].PutValue("Sample HTML Export");
            
            // Создайте параметры сохранения HTML и установите ExportDocumentProperties в false
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportDocumentProperties = false;
            
            // Сохраните книгу в формате HTML
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML file saved with document properties export disabled.");
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


