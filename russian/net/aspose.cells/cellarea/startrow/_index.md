---
title: "CellArea.StartRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Поле CellArea. Получает или задает начальную строку этой области"
type: docs
url: /ru/net/aspose.cells/cellarea/startrow/
---
## CellArea.StartRow field

Получает или задаёт начальную строку этой области.

```csharp
public int StartRow;
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellAreaFieldStartRowDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте два объекта CellArea
            CellArea area1 = new CellArea();
            area1.StartRow = 2;
            area1.StartColumn = 1;
            area1.EndRow = 5;
            area1.EndColumn = 3;

            CellArea area2 = new CellArea();
            area2.StartRow = area1.StartRow; // Demonstrating StartRow usage
            area2.StartColumn = area1.StartColumn;
            area2.EndRow = area1.EndRow;
            area2.EndColumn = area1.EndColumn;

            // Проверьте, что области совпадают
            if (area1.StartRow == area2.StartRow &&
                area1.StartColumn == area2.StartColumn &&
                area1.EndRow == area2.EndRow &&
                area1.EndColumn == area2.EndColumn)
            {
                Console.WriteLine("CellArea objects match successfully");
                Console.WriteLine($"StartRow: {area1.StartRow}");
            }
            else
            {
                Console.WriteLine("CellArea objects do not match");
            }
        }
    }
}
```

### См. также

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


