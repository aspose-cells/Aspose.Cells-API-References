---
title: "Cells.MinRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cells. Минимальный индекс строки ячейки, содержащей данные или стиль"
type: docs
url: /ru/net/aspose.cells/cells/minrow/
---
## Cells.MinRow property

Минимальный индекс строки ячейки, содержащей данные или стиль.

```csharp
public int MinRow { get; }
```

### Примечания

Это свойство должно динамически проходить и проверять ячейки и строки, поэтому процесс затратный по времени и не должно вызываться многократно, например использовать его напрямую как условие в цикле.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMinRowDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Добавьте некоторые данные, чтобы продемонстрировать MinRow
            cells["A1"].PutValue("Data in first row");
            cells["B5"].PutValue("Data in fifth row");

            // Отобразить информацию о MinRow
            Console.WriteLine("Minimum used row: " + cells.MinRow);
            Console.WriteLine("Maximum used row: " + cells.MaxRow);

            // Очистить содержимое, начиная с MinRow
            cells.ClearContents(cells.MinRow, cells.MinColumn, cells.MaxRow, cells.MaxColumn);

            // Проверьте очистку, проверив, пусты ли ячейки
            Console.WriteLine("A1 after clearing: " + (cells["A1"].Value == null ? "Empty" : "Not empty"));
            Console.WriteLine("B5 after clearing: " + (cells["B5"].Value == null ? "Empty" : "Not empty"));
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


