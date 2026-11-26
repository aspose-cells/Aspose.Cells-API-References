---
title: "Перечисление TotalsCalculation"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Tables.TotalsCalculation. Определяет тип вычисления в строке Totals столбца списка"
type: docs
url: /ru/net/aspose.cells.tables/totalscalculation/
---
## TotalsCalculation enumeration

Определяет тип вычисления в строке Totals списка столбцов.

```csharp
public enum TotalsCalculation
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Sum | `6` | Представляет вычисление суммы. |
| Count | `2` | Представляет вычисление количества. |
| Average | `1` | Представляет вычисление среднего. |
| Max | `4` | Представляет вычисление максимума. |
| Min | `5` | Представляет вычисление итогов Min. |
| Var | `8` | Представляет вычисление итогов Var. |
| CountNums | `3` | Представляет вычисление итогов Count Nums. |
| StdDev | `7` | Представляет вычисление итогов StdDev. |
| None | `0` | Представляет вычисление итогов No. |
| Custom | `9` | Представляет пользовательское вычисление. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TotalsCalculationDemo
    {
        public static void TotalsCalculationExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Заполните лист некоторыми данными
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue(CellsHelper.ColumnIndexToName(i));
            }
            for (int row = 1; row < 10; row++)
            {
                for (int column = 0; column < 4; column++)
                {
                    cells[row, column].PutValue(row * column);
                }
            }

            // Добавить таблицу в лист
            ListObjectCollection tables = workbook.Worksheets[0].ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];

            // Показать строку итогов
            table.ShowTotals = true;

            // Получить доступ к пятой колонке в таблице
            ListColumn listColumn = table.ListColumns[4];

            // Установите свойство TotalsCalculation в Sum
            listColumn.TotalsCalculation = TotalsCalculation.Sum;

            // При необходимости задайте формулу для колонки
            listColumn.Formula = "=[A]";

            // Сохраните книгу
            workbook.Save("TotalsCalculationExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


