---
title: "Cell.IsNumericValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cell. Указывает, является ли значение этой ячейки числовым, целым, двойным или датой/временем"
type: docs
url: /ru/net/aspose.cells/cell/isnumericvalue/
---
## Cell.IsNumericValue property

Указывает, является ли значение этой ячейки числовым (int, double и datetime).

```csharp
public bool IsNumericValue { get; }
```

### Примечания

Также применяется к ячейке с формулой для проверки вычисленного результата

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsNumericValueDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте различные типы данных в ячейки
            Cell cell1 = worksheet.Cells["A1"];
            cell1.PutValue(123.45); // Numeric value

            Cell cell2 = worksheet.Cells["A2"];
            cell2.PutValue("Hello World"); // String value

            // Проверьте, содержат ли ячейки числовые значения
            Console.WriteLine("Cell A1 IsNumericValue: " + cell1.IsNumericValue);
            Console.WriteLine("Cell A2 IsNumericValue: " + cell2.IsNumericValue);

            // Продемонстрируйте использование с условной логикой
            if (cell1.IsNumericValue)
            {
                Console.WriteLine("Cell A1 contains a numeric value: " + cell1.DoubleValue);
            }

            if (!cell2.IsNumericValue)
            {
                Console.WriteLine("Cell A2 does not contain a numeric value");
            }
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


