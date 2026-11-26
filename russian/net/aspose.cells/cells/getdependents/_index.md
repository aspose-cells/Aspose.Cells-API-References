---
title: "Cells.GetDependents"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Получить все ячейки, которые ссылаются на указанную ячейку"
type: docs
url: /ru/net/aspose.cells/cells/getdependents/
---
## Cells.GetDependents method

Получить все ячейки, которые ссылаются на конкретную ячейку.

```csharp
public Cell[] GetDependents(bool isAll, int row, int column)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| isAll | Boolean | Указывает, следует ли проверять другие листы |
| строка | Int32 | Индекс строки. |
| column | Int32 | Индекс столбца. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetDependentsWithBooleanInt32Int32Demo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Настройте примерные формулы и значения
            cells["A1"].PutValue(10);
            cells["B1"].Formula = "=A1*2";
            cells["C1"].Formula = "=A1+B1";
            cells["D1"].Formula = "=B1*3";
            cells["F4"].Formula = "=A1*5";

            // Вычислить формулы
            workbook.CalculateFormula();

            // Получить прямые зависимости ячейки A1 (строка 0, столбец 0)
            Cell[] directDependents = cells.GetDependents(false, 0, 0);
            Console.WriteLine("Direct dependents of A1:");
            foreach (Cell cell in directDependents)
            {
                Console.WriteLine(cell.Name);
            }

            // Получить все зависимости (включая косвенные) ячейки A1 (строка 0, столбец 0)
            Cell[] allDependents = cells.GetDependents(true, 0, 0);
            Console.WriteLine("\nAll dependents of A1:");
            foreach (Cell cell in allDependents)
            {
                Console.WriteLine(cell.Name);
            }
        }
    }
}
```

### См. также

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


