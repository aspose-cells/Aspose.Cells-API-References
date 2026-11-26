---
title: "CellArea.StartColumn"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Поле CellArea. Получает или задает начальный столбец этой области"
type: docs
url: /ru/net/aspose.cells/cellarea/startcolumn/
---
## CellArea.StartColumn field

Получает или задаёт начальный столбец этой области.

```csharp
public int StartColumn;
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellAreaFieldStartColumnDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Установить некоторые начальные данные
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue(10);
            cells["A3"].PutValue(20);

            // Создать объект CellArea и задать его StartColumn
            CellArea area = new CellArea();
            area.StartRow = 1;
            area.EndRow = 3;
            area.StartColumn = 0; // Using StartColumn field
            area.EndColumn = 0;

            // Вставить новый столбец, сдвинув существующие ячейки вниз
            cells.InsertRange(area, ShiftType.Down);

            // Проверить результат
            Console.WriteLine("A1 value: " + cells["A1"].StringValue); // Should be empty
            Console.WriteLine("A2 value: " + cells["A2"].StringValue); // Should be "Header"
            Console.WriteLine("A3 value: " + cells["A3"].IntValue); // Should be 10
        }
    }
}
```

### См. также

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


