---
title: "HtmlSaveOptions.ExportPageHeaders"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Указывает, экспортируются ли заголовки страниц"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/exportpageheaders/
---
## HtmlSaveOptions.ExportPageHeaders property

Указывает, экспортировать ли заголовки страниц.

```csharp
public bool ExportPageHeaders { get; set; }
```

### Примечания

Работает только когда [`SaveAsSingleFile`](../saveassinglefile/) равно True.

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportPageHeadersDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установить заголовок страницы
            worksheet.PageSetup.SetHeader(0, "Sample Header Text");
            
            // Добавить некоторые данные в лист
            worksheet.Cells["A1"].PutValue("This is a test");
            
            // Настроить параметры сохранения HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                SaveAsSingleFile = true,
                ShowAllSheets = true,
                ExportPageHeaders = true  // This is the key property being demonstrated
            };
            
            // Сохраните книгу в формате HTML
            string outputPath = "output_with_headers.html";
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("HTML file with page headers exported successfully.");
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


