---
title: "HtmlSaveOptions.ExportSingleTab"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Указывает, экспортировать ли единственную вкладку, когда файл содержит только один лист. Значение по умолчанию — false."
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/exportsingletab/
---
## HtmlSaveOptions.ExportSingleTab property

Указывает, экспортировать ли единственную вкладку, когда файл содержит только один лист. Значение по умолчанию — false.

```csharp
public bool ExportSingleTab { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportSingleTabDemo
    {
        public static void Run()
        {
            // Создайте новую рабочую книгу с тестовыми данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Создайте параметры сохранения HTML с установленным ExportSingleTab в true.
            HtmlSaveOptions options = new HtmlSaveOptions
            {
                ExportSingleTab = true,
                ExportImagesAsBase64 = true
            };

            // Сохраните книгу в формате HTML
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "SingleTabExport.html");
            workbook.Save(outputPath, options);

            Console.WriteLine("HTML file with single tab export created successfully: " + outputPath);
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


