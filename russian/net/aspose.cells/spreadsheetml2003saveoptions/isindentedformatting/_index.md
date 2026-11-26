---
title: "SpreadsheetML2003SaveOptions.IsIndentedFormatting"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SpreadsheetML2003SaveOptions. Заставляет дочерние элементы быть отступленными"
type: docs
url: /ru/net/aspose.cells/spreadsheetml2003saveoptions/isindentedformatting/
---
## SpreadsheetML2003SaveOptions.IsIndentedFormatting property

Заставляет дочерние элементы быть с отступом.

```csharp
public bool IsIndentedFormatting { get; set; }
```

### Примечания

Значение по умолчанию — true. Если значение равно false, размер XML‑файла будет уменьшен

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpreadsheetML2003SaveOptionsPropertyIsIndentedFormattingDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);

            // Настройте параметры сохранения с отступным форматированием
            SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions
            {
                IsIndentedFormatting = true
            };

            // Сохранить с отступным форматированием XML
            workbook.Save("output_indented.xml", saveOptions);

            // Сохранить без отступного форматирования для сравнения
            saveOptions.IsIndentedFormatting = false;
            workbook.Save("output_not_indented.xml", saveOptions);
        }
    }
}
```

### См. также

* class [SpreadsheetML2003SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


