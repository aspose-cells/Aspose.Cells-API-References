---
title: "DeleteBlankOptions.EndIndex"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DeleteBlankOptions. Указывает конечный индекс строки/столбца, включительно диапазон, который необходимо проверить и удалить пустые строки/столбцы. Значение по умолчанию — 1, а 1 означает максимальный диапазон всех объектов, ячеек, рисунков ... которые нужно проверить."
type: docs
url: /ru/net/aspose.cells/deleteblankoptions/endindex/
---
## DeleteBlankOptions.EndIndex property

Задает конечный индекс строки/столбца (включительно) диапазона, который нужно проверить и удалить пустые строки/столбцы. Значение по умолчанию — -1, а -1 означает максимальный диапазон всех объектов (ячейки, рисунки, ...) которые необходимо проверить.

```csharp
public int EndIndex { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteBlankOptionsPropertyEndIndexDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;

            // Заполните некоторые ячейки значениями
            cells[0, 2].PutValue(2);
            cells[0, 5].PutValue(5);
            cells[0, 9].PutValue(9);

            // Создайте параметры удаления с определённым диапазоном
            DeleteBlankOptions dbo = new DeleteBlankOptions();
            dbo.StartIndex = 4;
            dbo.EndIndex = 7;

            // Удалите пустые столбцы в указанном диапазоне
            cells.DeleteBlankColumns(dbo);

            // Выведите результаты, чтобы продемонстрировать влияние EndIndex
            Console.WriteLine("Value at C1: " + cells[0, 2].IntValue);
            Console.WriteLine("Value at F1 (originally G1): " + cells[0, 4].IntValue);
            Console.WriteLine("Value at G1 (originally K1): " + cells[0, 6].IntValue);
        }
    }
}
```

### См. также

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


