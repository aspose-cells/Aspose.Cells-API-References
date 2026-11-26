---
title: "Cell.GetStringValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cell. Получает строковое значение с помощью конкретной стратегии форматирования"
type: docs
url: /ru/net/aspose.cells/cell/getstringvalue/
---
## Cell.GetStringValue method

Получает строковое значение по определённой стратегии форматирования.

```csharp
public string GetStringValue(CellValueFormatStrategy formatStrategy)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| formatStrategy | CellValueFormatStrategy | Отформатированная стратегия. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetStringValueWithCellValueFormatStrategyDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Установите различные типы данных в ячейках
            cells["A1"].PutValue(123.45); // Numeric value
            cells["A2"].PutValue(DateTime.Now); // DateTime value
            cells["A3"].PutValue(true); // Boolean value
            cells["A4"].PutValue("Sample Text"); // String value

            // Продемонстрировать GetStringValue с различными стратегиями форматирования
            Console.WriteLine("None: " + cells["A1"].GetStringValue(CellValueFormatStrategy.None));
            Console.WriteLine("CellStyle: " + cells["A1"].GetStringValue(CellValueFormatStrategy.CellStyle));
            Console.WriteLine("DisplayString: " + cells["A1"].GetStringValue(CellValueFormatStrategy.DisplayString));

            Console.WriteLine("DateTime None: " + cells["A2"].GetStringValue(CellValueFormatStrategy.None));
            Console.WriteLine("DateTime CellStyle: " + cells["A2"].GetStringValue(CellValueFormatStrategy.CellStyle));
        }
    }
}
```

### См. также

* enum [CellValueFormatStrategy](../../cellvalueformatstrategy/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


