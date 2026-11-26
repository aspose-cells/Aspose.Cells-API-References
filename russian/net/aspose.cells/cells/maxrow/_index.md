---
title: "Cells.MaxRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cells. Максимальный индекс строки ячейки, содержащей данные или стиль"
type: docs
url: /ru/net/aspose.cells/cells/maxrow/
---
## Cells.MaxRow property

Максимальный индекс строки ячейки, содержащей данные или стиль.

```csharp
public int MaxRow { get; }
```

### Примечания

Возвращает -1, если в листе нет ячейки, содержащей данные или стиль. Это свойство требует итерации и динамической проверки ячеек и строк, поэтому процесс затратный по времени и не должно вызываться многократно, например, использовать его напрямую в условии цикла.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMaxRowDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Добавьте некоторые образцы данных.
            cells[0, 0].PutValue("Name");
            cells[0, 1].PutValue("Age");
            cells[1, 0].PutValue("John");
            cells[1, 1].PutValue(30);
            cells[2, 0].PutValue("Alice");
            cells[2, 1].PutValue(25);

            // Получить максимальный индекс строки (нумерация с нуля)
            int maxRow = cells.MaxRow;
            Console.WriteLine("MaxRow before adding new data: " + maxRow);

            // Добавить новые данные в следующую строку после максимальной строки
            int newRow = maxRow + 1;
            cells[newRow, 0].PutValue("Bob");
            cells[newRow, 1].PutValue(28);

            // Проверить новую максимальную строку
            Console.WriteLine("MaxRow after adding new data: " + cells.MaxRow);

            // Сохраните книгу
            workbook.Save("MaxRowDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


