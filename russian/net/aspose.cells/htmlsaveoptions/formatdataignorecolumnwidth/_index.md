---
title: "HtmlSaveOptions.FormatDataIgnoreColumnWidth"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Указывает, показывать ли полностью отформатированные данные ячейки при переполнении столбца. Если true, ширина столбца игнорируется, и все данные ячейки экспортируются. Если false, данные экспортируются так же, как в Excel. Значение по умолчанию — false."
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/formatdataignorecolumnwidth/
---
## HtmlSaveOptions.FormatDataIgnoreColumnWidth property

Указывает, показывать ли полностью отформатированные данные ячейки при переполнении столбца. Если true, ширина столбца игнорируется и экспортируются все данные ячейки. Если false, данные экспортируются так же, как в Excel. Значение по умолчанию — false.

```csharp
public bool FormatDataIgnoreColumnWidth { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyFormatDataIgnoreColumnWidthDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установите примерные данные и ширину столбца.
            worksheet.Cells["A1"].PutValue("Sample Text");
            worksheet.Cells["B1"].PutValue("Longer Text That Might Be Truncated");
            worksheet.Cells.SetColumnWidth(0, 10); // Narrow column
            worksheet.Cells.SetColumnWidth(1, 5);  // Very narrow column

            // Создать параметры сохранения HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Продемонстрируйте свойство FormatDataIgnoreColumnWidth.
            saveOptions.FormatDataIgnoreColumnWidth = true; // Text won't be truncated by column width
            
            // Сохраните с разными настройками, чтобы показать эффект.
            workbook.Save("HtmlWithIgnoreColumnWidth.html", saveOptions);
            
            saveOptions.FormatDataIgnoreColumnWidth = false; // Text may be truncated by column width
            workbook.Save("HtmlWithoutIgnoreColumnWidth.html", saveOptions);
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


