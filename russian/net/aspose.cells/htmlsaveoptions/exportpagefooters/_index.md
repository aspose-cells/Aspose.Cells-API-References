---
title: "HtmlSaveOptions.ExportPageFooters"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Указывает, экспортируются ли заголовки страниц"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/exportpagefooters/
---
## HtmlSaveOptions.ExportPageFooters property

Указывает, экспортировать ли заголовки страниц.

```csharp
public bool ExportPageFooters { get; set; }
```

### Примечания

Работает только когда [`SaveAsSingleFile`](../saveassinglefile/) равно True.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportPageFootersDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // Создать параметры сохранения HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Установите ExportPageFooters в true, чтобы включить нижние колонтитулы страниц в вывод
            saveOptions.ExportPageFooters = true;
            
            // Установите другие необходимые параметры
            saveOptions.ExportPageHeaders = true;
            
            // Сохраните книгу в HTML
            workbook.Save("HtmlWithPageFooters.html", saveOptions);
            
            Console.WriteLine("HTML file with page footers exported successfully.");
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


