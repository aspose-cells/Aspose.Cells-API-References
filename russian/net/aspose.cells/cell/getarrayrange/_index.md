---
title: "Cell.GetArrayRange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cell. Получает диапазон массива, если формула ячейки является массивной формулой"
type: docs
url: /ru/net/aspose.cells/cell/getarrayrange/
---
## Cell.GetArrayRange method

Получает диапазон массива, если формула ячейки является массивной формулой.

```csharp
public CellArea GetArrayRange()
```

### Возвращаемое значение

Диапазон массива.

### Примечания

Применяется только когда формула ячейки является массивной формулой

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetArrayRangeDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Установите динамическую массивную формулу в ячейку A1
            Cell cell = cells[0, 0];
            string formula = "=SEQUENCE(3,2)";
            cell.SetDynamicArrayFormula(formula, new FormulaParseOptions(), false);
            
            // Вычислить формулы
            wb.CalculateFormula();
            
            // Получить диапазон массива динамической формулы
            CellArea arrayRange = cell.GetArrayRange();
            
            // Вывести информацию о диапазоне массива
            Console.WriteLine("Array range for dynamic formula:");
            Console.WriteLine($"Start row: {arrayRange.StartRow}");
            Console.WriteLine($"Start column: {arrayRange.StartColumn}");
            Console.WriteLine($"End row: {arrayRange.EndRow}");
            Console.WriteLine($"End column: {arrayRange.EndColumn}");
            
            // Напечатать значения в диапазоне массива
            Console.WriteLine("\nValues in the array range:");
            for (int r = arrayRange.StartRow; r <= arrayRange.EndRow; r++)
            {
                for (int c = arrayRange.StartColumn; c <= arrayRange.EndColumn; c++)
                {
                    Console.Write(cells[r, c].Value + "\t");
                }
                Console.WriteLine();
            }
        }
    }
}
```

### См. также

* struct [CellArea](../../cellarea/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


