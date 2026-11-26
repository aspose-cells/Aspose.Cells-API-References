---
title: "Перечисление MergedCellsShrinkType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.MergedCellsShrinkType. Представляет стратегию сжатия объединённых ячеек для операций, таких как удаление пустых строк/столбцов"
type: docs
url: /ru/net/aspose.cells/mergedcellsshrinktype/
---
## MergedCellsShrinkType enumeration

Представляет стратегию сжатия объединённых ячеек для операций, таких как удаление пустых строк/столбцов.

```csharp
public enum MergedCellsShrinkType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` | Оставляет объединённые ячейки без каких-либо изменений. |
| ShrinkToFit | `1` | Сжимает объединённую область при необходимости, удаляя строки снизу или столбцы справа, при этом обеспечивая видимость всего содержимого. |
| KeepHeaderOnly | `2` | Сохраняет только строки/столбцы заголовка объединённой области, если верхняя левая ячейка этой области не пустая. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassMergedCellsShrinkTypeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            Cells cells = ws.Cells;

            // Инициализировать пример данных с объединёнными ячейками
            cells.Merge(0, 0, 1, 2);
            cells[0, 0].PutValue("Merged Header");
            cells[1, 2].PutValue("Data 1");
            cells[2, 2].PutValue("Data 2");

            Console.WriteLine("Original worksheet:");
            PrintCellValues(cells);

            // Вариант 1: KeepHeaderOnly
            DeleteBlankOptions opts1 = new DeleteBlankOptions();
            opts1.MergedCellsShrinkType = MergedCellsShrinkType.KeepHeaderOnly;
            cells.DeleteBlankColumns(opts1);
            Console.WriteLine("\nAfter DeleteBlankColumns with KeepHeaderOnly:");
            PrintCellValues(cells);

            // Сбросить лист
            cells.ClearContents(0, 0, cells.MaxDataRow, cells.MaxDataColumn);
            cells.Merge(0, 0, 1, 2);
            cells[0, 0].PutValue("Merged Header");
            cells[1, 2].PutValue("Data 1");
            cells[2, 2].PutValue("Data 2");

            // Вариант 2: None
            DeleteBlankOptions opts2 = new DeleteBlankOptions();
            opts2.MergedCellsShrinkType = MergedCellsShrinkType.None;
            cells.DeleteBlankColumns(opts2);
            Console.WriteLine("\nAfter DeleteBlankColumns with None:");
            PrintCellValues(cells);

            // Сбросить лист
            cells.ClearContents(0, 0, cells.MaxDataRow, cells.MaxDataColumn);
            cells.Merge(0, 0, 1, 2);
            cells[0, 0].PutValue("Merged Header");
            cells[1, 2].PutValue("Data 1");
            cells[2, 2].PutValue("Data 2");

            // Вариант 3: ShrinkToFit
            DeleteBlankOptions opts3 = new DeleteBlankOptions();
            opts3.MergedCellsShrinkType = MergedCellsShrinkType.ShrinkToFit;
            cells.DeleteBlankColumns(opts3);
            Console.WriteLine("\nAfter DeleteBlankColumns with ShrinkToFit:");
            PrintCellValues(cells);
        }

        private static void PrintCellValues(Cells cells)
        {
            for (int row = 0; row < 3; row++)
            {
                for (int col = 0; col < 3; col++)
                {
                    Console.Write($"({row},{col}): {cells[row, col].Value ?? "empty"} | ");
                }
                Console.WriteLine();
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


