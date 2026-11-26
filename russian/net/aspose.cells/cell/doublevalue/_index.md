---
title: "Cell.DoubleValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cell. Возвращает двойное значение, содержащееся в ячейке"
type: docs
url: /ru/net/aspose.cells/cell/doublevalue/
---
## Cell.DoubleValue property

Получает значение double, содержащееся в ячейке.

```csharp
public double DoubleValue { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyDoubleValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Установите различные типы значений в ячейках
            cells["A1"].PutValue(1); // Int value
            cells["A2"].PutValue(true); // Bool value
            cells["A3"].PutValue("abc"); // String value
            cells["A4"].PutValue(false); // Bool value
            cells["A5"].PutValue(2.56); // Double value

            // Продемонстрировать свойство DoubleValue
            Console.WriteLine("Double value from cell A5: " + cells["A5"].DoubleValue);
            
            // Проверьте, что другие типы значений могут быть прочитаны как double
            Console.WriteLine("Int as double from A1: " + cells["A1"].DoubleValue);
            Console.WriteLine("Bool as double from A2: " + cells["A2"].DoubleValue);
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


