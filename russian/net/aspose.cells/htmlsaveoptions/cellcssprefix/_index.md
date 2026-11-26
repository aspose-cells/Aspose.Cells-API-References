---
title: "HtmlSaveOptions.CellCssPrefix"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Получает и задает префикс имени CSS. Значение по умолчанию —"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/cellcssprefix/
---
## HtmlSaveOptions.CellCssPrefix property

Получает и задаёт префикс имени CSS, значение по умолчанию — \"\".

```csharp
public string CellCssPrefix { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyCellCssPrefixDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в ячейки
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);

            // Установите параметры сохранения HTML с CellCssPrefix
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.CellCssPrefix = "custom-cell-";

            // Сохранить рабочую книгу с параметрами HTML
            workbook.Save("output.html", saveOptions);

            Console.WriteLine("HTML file saved with custom cell CSS prefix.");
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


