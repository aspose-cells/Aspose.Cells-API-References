---
title: "HtmlSaveOptions.ExportExtraHeadings"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Указывает, экспортировать ли дополнительные заголовки, когда длина текста превышает максимальную отображаемую колонку. Значение по умолчанию — false. Если вы хотите импортировать html‑файл в Excel, пожалуйста, оставьте значение по умолчанию."
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/exportextraheadings/
---
## HtmlSaveOptions.ExportExtraHeadings property

Указывает, экспортировать ли дополнительные заголовки, когда длина текста превышает максимальную отображаемую колонку. Значение по умолчанию — false. Если вы хотите импортировать html‑файл в Excel, пожалуйста, оставьте значение по умолчанию.

```csharp
public bool ExportExtraHeadings { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportExtraHeadingsDemo
    {
        public static void Run()
        {
            // Создать новую книгу с примерными данными.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить пример данных и дополнительные заголовки
            worksheet.Cells["A1"].PutValue("Main Heading");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            worksheet.Cells["A3"].PutValue("Data3");
            worksheet.Cells["B3"].PutValue("Data4");
            
            // Установить дополнительные заголовки (строки и столбцы)
            worksheet.Cells["Z1"].PutValue("Extra Column Heading");
            worksheet.Cells["A100"].PutValue("Extra Row Heading");

            // Настроить параметры сохранения HTML с ExportExtraHeadings
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportHeadings = true;
            saveOptions.ExportExtraHeadings = true;

            // Сохранить в HTML
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("HTML exported with extra headings.");
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


