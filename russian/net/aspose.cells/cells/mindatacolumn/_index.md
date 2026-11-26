---
title: "Cells.MinDataColumn"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cells. Минимальный индекс столбца ячейки, содержащей данные"
type: docs
url: /ru/net/aspose.cells/cells/mindatacolumn/
---
## Cells.MinDataColumn property

Минимальный индекс столбца ячейки, содержащей данные.

```csharp
public int MinDataColumn { get; }
```

### Примечания

-1 will be returned if there is no cell which contains data. This property needs to iterate and check all cells in a worksheet dynamically, so it is a time-consumed progress and should not be invoked repeatedly, such as using it directly as condition in a loop.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMinDataColumnDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Добавьте некоторые данные в ячейки (начиная со столбца 2)
            cells["B1"].PutValue("Header1");
            cells["C2"].PutValue("Data1");
            cells["D3"].PutValue("Data2");
            cells["E4"].PutValue("Data3");
            
            // Получите минимальный индекс столбца, содержащего данные.
            int minDataColumn = cells.MinDataColumn;
            
            // Вывести результат.
            Console.WriteLine("Minimum data column index: " + minDataColumn);
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


