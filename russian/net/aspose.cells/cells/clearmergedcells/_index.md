---
title: "Cells.ClearMergedCells"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Очищает все объединённые диапазоны"
type: docs
url: /ru/net/aspose.cells/cells/clearmergedcells/
---
## Cells.ClearMergedCells method

Очищает все объединённые диапазоны.

```csharp
public void ClearMergedCells()
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodClearMergedCellsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать объединённые ячейки в диапазоне A1:B2
            worksheet.Cells.Merge(0, 0, 2, 2);
            Console.WriteLine($"Merged areas before clearing: {worksheet.Cells.GetMergedAreas().Length}");

            try
            {
                // Очистить все объединённые ячейки в листе
                worksheet.Cells.ClearMergedCells();
                Console.WriteLine("Method executed successfully");
                Console.WriteLine($"Merged areas after clearing: {worksheet.Cells.GetMergedAreas().Length}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearMergedCells method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("ClearMergedCellsDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


