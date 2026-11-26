---
title: "HtmlSaveOptions.ExportBogusRowData"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Указывает, экспортировать ли фиктивные данные нижней строки. Значение по умолчанию — true. Если вы хотите импортировать HTML или MHT файл в Excel, пожалуйста, оставьте значение по умолчанию"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/exportbogusrowdata/
---
## HtmlSaveOptions.ExportBogusRowData property

Указывает, экспортировать ли фиктивные данные нижней строки. Значение по умолчанию — true.If вы хотите импортировать файл html или mht в Excel, пожалуйста, оставьте значение по умолчанию.

```csharp
public bool ExportBogusRowData { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportBogusRowDataDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте некоторые данные в ячейки
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);

            // Создать параметры сохранения HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
            
            // Первый экспорт без фиктивных данных строки
            saveOptions.ExportBogusRowData = false;
            workbook.Save("output_without_bogus.html", saveOptions);
            
            // Затем экспорт с фиктивными данными строки
            saveOptions.ExportBogusRowData = true;
            workbook.Save("output_with_bogus.html", saveOptions);

            // Отобразите результаты
            Console.WriteLine("HTML files created successfully.");
            Console.WriteLine("Check output_without_bogus.html and output_with_bogus.html to see the difference.");
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


