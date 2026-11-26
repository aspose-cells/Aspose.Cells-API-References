---
title: "DeleteBlankOptions.StartIndex"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DeleteBlankOptions. Указывает начальный индекс строки/столбца диапазона, который следует проверить и удалить пустую строку/столбец"
type: docs
url: /ru/net/aspose.cells/deleteblankoptions/startindex/
---
## DeleteBlankOptions.StartIndex property

Задает начальный индекс строки/столбца диапазона, который нужно проверить и удалить пустую строку/столбец.

```csharp
public int StartIndex { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteBlankOptionsPropertyStartIndexDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Заполните некоторые ячейки значениями
            cells[2, 0].PutValue("Row 3");
            cells[5, 0].PutValue("Row 6");
            cells[9, 0].PutValue("Row 10");

            Console.WriteLine("Before deleting blank rows:");
            for (int i = 0; i <= 10; i++)
            {
                Console.WriteLine($"Row {i + 1}: {(cells[i, 0].Value ?? "empty")}");
            }

            // Удалить пустые строки, начиная с индекса 4 (строка 5) до индекса 7 (строка 8)
            DeleteBlankOptions options = new DeleteBlankOptions();
            options.StartIndex = 4;
            options.EndIndex = 7;
            cells.DeleteBlankRows(options);

            Console.WriteLine("\nAfter deleting blank rows from Row 5 to Row 8:");
            for (int i = 0; i <= 7; i++)
            {
                Console.WriteLine($"Row {i + 1}: {(cells[i, 0].Value ?? "empty")}");
            }
        }
    }
}
```

### См. также

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


