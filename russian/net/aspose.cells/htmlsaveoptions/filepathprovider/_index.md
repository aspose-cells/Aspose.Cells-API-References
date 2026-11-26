---
title: "HtmlSaveOptions.FilePathProvider"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Получает или задает IFilePathProvider для отдельного экспорта листа Worksheet в html."
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/filepathprovider/
---
## HtmlSaveOptions.FilePathProvider property

Получает или задает IFilePathProvider для отдельного экспорта листа в html.

```csharp
public IFilePathProvider FilePathProvider { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyFilePathProviderDemo
    {
        public static void Run()
        {
            // Создать новую книгу и добавить некоторые данные
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");

            // Создать HtmlSaveOptions и установить FilePathProvider
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.FilePathProvider = new CustomFilePathProvider();

            // Сохраните книгу в формате HTML
            workbook.Save("output.html", saveOptions);

            Console.WriteLine("Workbook saved to HTML with custom file paths.");
        }
    }

    public class CustomFilePathProvider : IFilePathProvider
    {
        public string GetFullName(string sheetName)
        {
            // Пользовательская логика для генерации путей к файлам
            return $"custom_{sheetName}";
        }
    }
}
```

### См. также

* interface [IFilePathProvider](../../ifilepathprovider/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


