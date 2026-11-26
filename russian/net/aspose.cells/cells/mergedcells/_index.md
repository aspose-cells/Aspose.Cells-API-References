---
title: "Cells.MergedCells"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cells. Возвращает коллекцию объединённых ячеек"
type: docs
url: /ru/net/aspose.cells/cells/mergedcells/
---
## Cells.MergedCells property

Возвращает коллекцию объединённых ячеек.

```csharp
[Obsolete("Use Cells.GetMergedAreas() instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList MergedCells { get; }
```

### Примечания

В этой коллекции каждый элемент представляет собой структуру [`CellArea`](../../cellarea/), которая описывает область объединённых ячеек.

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод Cells.GetMergedAreas(). Этот метод будет удалён через 12 месяцев, начиная с ноября 2023 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellsPropertyMergedCellsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Объединить ячейки в двух разных диапазонах
            cells.Merge(0, 0, 2, 2); // Merges A1:B2
            cells.Merge(2, 2, 2, 2); // Merges C3:D4

            // Получить доступ к свойству MergedCells (только для чтения)
            ArrayList mergedRanges = cells.MergedCells;

            // Отобразить начальное количество объединённых ячеек и их диапазоны
            Console.WriteLine($"Initial merged cells count: {mergedRanges.Count}");
            foreach (CellArea area in mergedRanges)
            {
                Console.WriteLine($"Merged area: Row[{area.StartRow}-{area.EndRow}], Column[{area.StartColumn}-{area.EndColumn}]");
            }

            // Разъединить первый объединённый диапазон
            cells.UnMerge(0, 0, 2, 2);

            // Отобразить обновлённое количество объединённых ячеек и их диапазоны
            Console.WriteLine($"\nAfter unmerging A1:B2 - Merged cells count: {cells.MergedCells.Count}");
            foreach (CellArea area in cells.MergedCells)
            {
                Console.WriteLine($"Remaining merged area: Row[{area.StartRow}-{area.EndRow}], Column[{area.StartColumn}-{area.EndColumn}]");
            }

            // Сохранить результат
            workbook.Save("PropertyMergedCellsDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


