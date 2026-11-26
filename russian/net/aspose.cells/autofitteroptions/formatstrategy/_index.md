---
title: "AutoFitterOptions.FormatStrategy"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство AutoFitterOptions. Получает и задает стратегию форматирования"
type: docs
url: /ru/net/aspose.cells/autofitteroptions/formatstrategy/
---
## AutoFitterOptions.FormatStrategy property

Получает и задает стратегию форматирования.

```csharp
public CellValueFormatStrategy FormatStrategy { get; set; }
```

### Примечания

Значение по умолчанию — CellStyle для повышения производительности.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyFormatStrategyDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установите примерные данные и включите перенос текста
            worksheet.Cells["A1"].PutValue("Sample text for FormatStrategy demo");
            Style style = worksheet.Cells["A1"].GetStyle();
            style.IsTextWrapped = true;
            worksheet.Cells["A1"].SetStyle(style);

            // Создайте AutoFitterOptions с FormatStrategy
            AutoFitterOptions options = new AutoFitterOptions
            {
                FormatStrategy = CellValueFormatStrategy.DisplayString,
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine
            };

            // Примените автоподгонку с указанными параметрами
            worksheet.AutoFitRows(options);

            // Сохранить результат
            workbook.Save("FormatStrategyDemo.xlsx");
        }
    }
}
```

### См. также

* enum [CellValueFormatStrategy](../../cellvalueformatstrategy/)
* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


