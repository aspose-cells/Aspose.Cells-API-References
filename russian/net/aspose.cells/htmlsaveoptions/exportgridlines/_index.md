---
title: "HtmlSaveOptions.ExportGridLines"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Указывает, экспортировать ли линии сетки. Значение по умолчанию — false"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/exportgridlines/
---
## HtmlSaveOptions.ExportGridLines property

Указывает, экспортировать ли линии сетки.Значение по умолчанию — false.

```csharp
public bool ExportGridLines { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportGridLinesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установить видимость линий сетки
            worksheet.IsGridlinesVisible = true;

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B2"].PutValue(123);
            worksheet.Cells["C3"].PutValue(DateTime.Now);

            // Создать параметры сохранения HTML
            HtmlSaveOptions options = new HtmlSaveOptions
            {
                ExportGridLines = worksheet.IsGridlinesVisible,
                ExportActiveWorksheetOnly = true
            };

            // Сохранить как HTML
            workbook.Save("output.html", options);

            Console.WriteLine("HTML file saved with ExportGridLines: " + options.ExportGridLines);
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


