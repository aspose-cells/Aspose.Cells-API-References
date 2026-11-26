---
title: "Cells.MinColumn"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cells. Минимальный индекс столбца тех ячеек, которые были созданы в коллекции, не включает столбец, в котором стиль определён для всего столбца, но ни одна ячейка в нём не была создана."
type: docs
url: /ru/net/aspose.cells/cells/mincolumn/
---
## Cells.MinColumn property

Минимальный индекс столбца среди ячеек, которые были созданы в коллекции (не включает столбец, в котором стиль определён для всего столбца, но ни одна ячейка в нём не создана).

```csharp
public int MinColumn { get; }
```

### Примечания

Это свойство должно динамически проходить и проверять ячейки и строки, поэтому процесс затратный по времени и не должно вызываться многократно, например использовать его напрямую как условие в цикле.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMinColumnDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Доступ к коллекции cells
            Cells cells = worksheet.Cells;
            
            // Заполните некоторые данные в столбцах 2, 3 и 4 (B, C, D).
            cells["B1"].PutValue("Data in Column B");
            cells["C1"].PutValue("Data in Column C");
            cells["D1"].PutValue("Data in Column D");
            
            // Получите минимальный индекс столбца, содержащего данные.
            int minColumn = cells.MinColumn;
            
            // Получите максимальный индекс столбца, содержащего данные.
            int maxColumn = cells.MaxColumn;
            
            Console.WriteLine("Minimum column with data: " + minColumn); // Should output 1 (column B)
            Console.WriteLine("Maximum column with data: " + maxColumn); // Should output 3 (column D)
            
            // Очистите столбец B, чтобы продемонстрировать изменение MinColumn.
            cells.DeleteColumn(1);
            
            Console.WriteLine("\nAfter deleting column B:");
            Console.WriteLine("New minimum column with data: " + cells.MinColumn); // Should now output 2 (column C)
            Console.WriteLine("Maximum column with data: " + cells.MaxColumn); // Should still output 3 (column D)
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


