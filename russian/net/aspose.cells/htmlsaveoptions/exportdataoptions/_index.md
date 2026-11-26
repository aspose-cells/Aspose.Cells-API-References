---
title: "HtmlSaveOptions.ExportDataOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "HtmlSaveOptions property. Указывает правило экспорта данных HTML‑файла. Значение по умолчанию — All"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/exportdataoptions/
---
## HtmlSaveOptions.ExportDataOptions property

Указывает правило экспорта данных html‑файла.Значение по умолчанию — All.

```csharp
public HtmlExportDataOptions ExportDataOptions { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportDataOptionsDemo
    {
        public static void Run()
        {
            // Создать пример рабочей книги с тестовыми данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Создайте параметры сохранения HTML и задайте ExportDataOptions
            HtmlSaveOptions htmlSaveOptions = new HtmlSaveOptions();
            htmlSaveOptions.ExportDataOptions = HtmlExportDataOptions.All;

            // Сохраните как HTML со всеми параметрами экспорта данных
            workbook.Save("output.html", htmlSaveOptions);

            Console.WriteLine("HTML file saved with ExportDataOptions.All");
        }
    }
}
```

### См. также

* enum [HtmlExportDataOptions](../../htmlexportdataoptions/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


