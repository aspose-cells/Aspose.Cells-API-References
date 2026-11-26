---
title: "Cells.MaxColumn"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cells. Максимальный индекс столбца тех ячеек, которые были созданы в коллекции, не включает столбец, в котором стиль определён для всего столбца, но ни одна ячейка в нём не была создана."
type: docs
url: /ru/net/aspose.cells/cells/maxcolumn/
---
## Cells.MaxColumn property

Максимальный индекс столбца среди ячеек, которые были созданы в коллекции (не включает столбец, в котором стиль определён для всего столбца, но ни одна ячейка в нём не создана).

```csharp
public int MaxColumn { get; }
```

### Примечания

Верните -1, если ни одна ячейка не была создана.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMaxColumnDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые данные в ячейки
            worksheet.Cells["A1"].PutValue("Column A");
            worksheet.Cells["B1"].PutValue("Column B");
            worksheet.Cells["C1"].PutValue("Column C");
            
            // Получите максимальный индекс столбца с данными.
            int maxColumn = worksheet.Cells.MaxColumn;
            Console.WriteLine("Max column with data: " + maxColumn);

            // Добавьте данные в следующий столбец после максимального столбца.
            worksheet.Cells[0, maxColumn + 1].PutValue("Next Column");

            // Проверьте новый максимальный столбец.
            Console.WriteLine("New max column: " + worksheet.Cells.MaxColumn);

            // Создайте другой лист для демонстрации копирования.
            Worksheet destSheet = workbook.Worksheets.Add("Destination");

            // Скопируйте все столбцы из источника в назначение.
            destSheet.Cells.CopyColumns(worksheet.Cells, 0, 0, worksheet.Cells.MaxColumn + 1);

            Console.WriteLine("Columns copied successfully");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


