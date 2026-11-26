---
title: "HtmlSaveOptions.ExportRowColumnHeadings"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Указывает, экспортировать ли заголовки строк и столбцов листов при сохранении в HTML‑файлы"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/exportrowcolumnheadings/
---
## HtmlSaveOptions.ExportRowColumnHeadings property

Указывает, экспортировать ли заголовки строк и столбцов листа при сохранении в HTML‑файлы.

```csharp
public bool ExportRowColumnHeadings { get; set; }
```

### Примечания

Значение по умолчанию — false.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportRowColumnHeadingsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в ячейки
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(15);

            // Создать параметры сохранения HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Установите ExportRowColumnHeadings в false (по умолчанию true)
            saveOptions.ExportRowColumnHeadings = false;

            // Сохранить книгу с отключенными заголовками
            workbook.Save("output_without_headings.html", saveOptions);

            // Теперь включите заголовки и сохраните снова
            saveOptions.ExportRowColumnHeadings = true;
            workbook.Save("output_with_headings.html", saveOptions);

            Console.WriteLine("HTML files saved with different heading visibility settings.");
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


