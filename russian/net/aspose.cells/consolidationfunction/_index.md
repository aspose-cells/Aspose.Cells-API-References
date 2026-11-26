---
title: "Перечисление ConsolidationFunction"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.ConsolidationFunction. Представляет функцию консолидации"
type: docs
url: /ru/net/aspose.cells/consolidationfunction/
---
## ConsolidationFunction enumeration

Представляет функцию консолидации.

```csharp
public enum ConsolidationFunction
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Sum | `0` | Представляет функцию Sum. |
| Count | `1` | Представляет функцию Count. |
| Average | `2` | Представляет функцию Average. |
| Max | `3` | Представляет функцию Max. |
| Min | `4` | Представляет функцию Min. |
| Product | `5` | Представляет функцию Product. |
| CountNums | `6` | Представляет функцию Count Nums. |
| StdDev | `7` | Представляет функцию StdDev. |
| StdDevp | `8` | Представляет функцию StdDevp. |
| Var | `9` | Представляет функцию Var. |
| Varp | `10` | Представляет функцию Varp. |
| DistinctCount | `11` | Представляет функцию Distinct Count. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConsolidationFunctionDemo
    {
        public static void ConsolidationFunctionExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Добавить новый лист в книгу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в лист
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Определите область ячеек для подытога
            CellArea cellArea = new CellArea
            {
                StartRow = 1,
                StartColumn = 0,
                EndRow = 3,
                EndColumn = 1
            };

            // Применить подытог с функцией Sum
            worksheet.Cells.Subtotal(cellArea, 0, ConsolidationFunction.Sum, new int[] { 1 });

            // Применить подытог с функцией Average
            worksheet.Cells.Subtotal(cellArea, 0, ConsolidationFunction.Average, new int[] { 1 });

            // Применить подытог с функцией Max
            worksheet.Cells.Subtotal(cellArea, 0, ConsolidationFunction.Max, new int[] { 1 });

            // Применить подытог с функцией Min
            worksheet.Cells.Subtotal(cellArea, 0, ConsolidationFunction.Min, new int[] { 1 });

            // Сохраните книгу
            workbook.Save("ConsolidationFunctionExample.xlsx");
            workbook.Save("ConsolidationFunctionExample.pdf");

            // Выведите результаты
            Console.WriteLine("Workbook saved with subtotals applied.");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


