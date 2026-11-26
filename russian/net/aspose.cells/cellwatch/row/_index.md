---
title: "CellWatch.Row"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CellWatch. Возвращает и задает строку ячейки"
type: docs
url: /ru/net/aspose.cells/cellwatch/row/
---
## CellWatch.Row property

Получает и задает строку ячейки.

```csharp
public int Row { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellWatchPropertyRowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить примерные данные в ячейку B2
            sheet.Cells["B2"].PutValue("Sample Data");

            // Добавить CellWatch для B2
            int watchIndex = sheet.CellWatches.Add("B2");
            CellWatch cellWatch = sheet.CellWatches[watchIndex];

            // Продемонстрировать свойство Row
            Console.WriteLine($"Original Row: {cellWatch.Row}");
            cellWatch.Row = 1; // Set row to 1 (0-based) for B2
            Console.WriteLine($"Updated Row: {cellWatch.Row}");

            // Проверьте ссылку на ячейку
            Console.WriteLine($"Cell Reference: {sheet.Cells[cellWatch.Row, cellWatch.Column].Name}");

            workbook.Save("CellWatchRowDemo.xlsx");
        }
    }
}
```

### См. также

* class [CellWatch](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


