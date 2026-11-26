---
title: "TxtSaveOptions.FormatStrategy"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TxtSaveOptions. Получает и задает стратегию форматирования при экспорте значения ячейки как строки"
type: docs
url: /ru/net/aspose.cells/txtsaveoptions/formatstrategy/
---
## TxtSaveOptions.FormatStrategy property

Получает и задает стратегию форматирования при экспорте значения ячейки как строки.

```csharp
public CellValueFormatStrategy FormatStrategy { get; set; }
```

### Примеры

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyFormatStrategyDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установить значения с разными форматами
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(999.99);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(599.99);

            // Применить числовой формат к ценам
            Style style = workbook.CreateStyle();
            style.Number = 2; // Format as currency
            worksheet.Cells["B2:B3"].SetStyle(style);

            // Настройте параметры сохранения текста с различными стратегиями форматирования
            TxtSaveOptions options = new TxtSaveOptions
            {
                Separator = '\t',
                FormatStrategy = CellValueFormatStrategy.DisplayStyle // Show formatted values
            };

            // Сохранить с отображаемым форматированием
            workbook.Save("FormattedOutput.txt", options);

            // Переключить на отсутствие стратегии форматирования
            options.FormatStrategy = CellValueFormatStrategy.None;
            workbook.Save("RawOutput.txt", options);

            Console.WriteLine("Files saved with different format strategies.");
        }
    }
}
```

### См. также

* enum [CellValueFormatStrategy](../../cellvalueformatstrategy/)
* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


