---
title: "Cell.IsErrorValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cell. Проверяет, является ли значение этой ячейки ошибкой"
type: docs
url: /ru/net/aspose.cells/cell/iserrorvalue/
---
## Cell.IsErrorValue property

Проверяет, является ли значение этой ячейки ошибкой.

```csharp
public bool IsErrorValue { get; }
```

### Примечания

Также применяется к ячейке с формулой для проверки, является ли вычисленный результат ошибкой.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsErrorValueDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Установите формулу, которая приведёт к ошибке
            Cell cell = cells["A1"];
            cell.Formula = "=1/0"; // Division by zero error
            
            // Вычислить формулы
            workbook.CalculateFormula();

            // Продемонстрируйте свойство IsErrorValue
            Console.WriteLine("Cell A1 value: " + cell.StringValue);
            Console.WriteLine("IsErrorValue: " + cell.IsErrorValue);
            Console.WriteLine("Error type: " + cell.Value);

            // Установите корректное значение
            Cell cell2 = cells["A2"];
            cell2.PutValue("Valid value");
            
            Console.WriteLine("\nCell A2 value: " + cell2.StringValue);
            Console.WriteLine("IsErrorValue: " + cell2.IsErrorValue);

            // Установить ошибку SPILL (ошибка формулы динамического массива в Excel 365+)
            Cell cell3 = cells["A3"];
            cell3.SetDynamicArrayFormula("=A1:A10", new FormulaParseOptions(), true);
            
            Console.WriteLine("\nCell A3 value: " + cell3.StringValue);
            Console.WriteLine("IsErrorValue: " + cell3.IsErrorValue);
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


