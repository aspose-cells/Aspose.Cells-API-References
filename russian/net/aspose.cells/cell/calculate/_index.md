---
title: "Cell.Calculate"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cell. Вычисляет формулу ячейки"
type: docs
url: /ru/net/aspose.cells/cell/calculate/
---
## Cell.Calculate method

Вычисляет формулу ячейки.

```csharp
public void Calculate(CalculationOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| опции | CalculationOptions | Параметры расчёта |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodCalculateWithCalculationOptionsDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установить простую формулу в ячейку A1
            Cell cellA1 = worksheet.Cells["A1"];
            cellA1.Formula = "=SUM(1, 2, 3)";
            
            // Вычислить с параметрами по умолчанию
            cellA1.Calculate(new CalculationOptions());
            Console.WriteLine("A1 value after calculation: " + cellA1.Value);

            // Установить массивную формулу в диапазоне B1:D1
            Cell cellB1 = worksheet.Cells["B1"];
            cellB1.SetArrayFormula("={1,2,3}", 1, 3);
            
            // Вычислить массивную формулу с параметрами
            cellB1.Calculate(new CalculationOptions());
            Console.WriteLine("B1 value after calculation: " + cellB1.Value);

            // Установить более сложную формулу в ячейку A2
            Cell cellA2 = worksheet.Cells["A2"];
            cellA2.Formula = "=IF(A1>5, \"Greater\", \"Less or equal\")";
            
            // Вычислить с параметрами
            cellA2.Calculate(new CalculationOptions());
            Console.WriteLine("A2 value after calculation: " + cellA2.Value);
        }
    }
}
```

### См. также

* class [CalculationOptions](../../calculationoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


