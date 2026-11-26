---
title: "HtmlSaveOptions.ExportPrintAreaOnly"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Указывает, экспортировать ли только область печати в html‑файл. Значение по умолчанию — false"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/exportprintareaonly/
---
## HtmlSaveOptions.ExportPrintAreaOnly property

Указывает, экспортировать ли только область печати в html‑файл. Значение по умолчанию — false.

```csharp
public bool ExportPrintAreaOnly { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportPrintAreaOnlyDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установить примерные данные
            for (int i = 0; i < 20; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Cell {i+1},{j+1}");
                }
            }

            // Установить область печати
            worksheet.PageSetup.PrintArea = "B2:F10";

            // Настроить параметры сохранения HTML
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportPrintAreaOnly = true;
            options.ExportGridLines = true;

            // Сохранить рабочую книгу только с областью печати
            workbook.Save("output.html", options);
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


