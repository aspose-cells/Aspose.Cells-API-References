---
title: "PageSetup.PrintHeadings"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PageSetup. Представляет, печатаются ли заголовки строк и столбцов на этой странице"
type: docs
url: /ru/net/aspose.cells/pagesetup/printheadings/
---
## PageSetup.PrintHeadings property

Отображает, печатаются ли заголовки строк и столбцов на этой странице.

```csharp
public bool PrintHeadings { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintHeadingsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установить некоторые образцы данных с заголовками
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1.8);

            // Включить печать заголовков
            worksheet.PageSetup.PrintHeadings = true;
            worksheet.PageSetup.PrintArea = "A1:B3";

            // Сохранить как HTML, чтобы продемонстрировать эффект
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                ExportActiveWorksheetOnly = true,
                ExportPrintAreaOnly = true,
                ExportGridLines = true,
                ExportHeadings = true
            };

            workbook.Save("PrintHeadingsDemo.html", saveOptions);

            Console.WriteLine("Worksheet saved with PrintHeadings enabled.");
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


