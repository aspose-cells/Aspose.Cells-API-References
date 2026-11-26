---
title: "Cell.IsMerged"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cell. Проверяет, является ли ячейка частью объединённого диапазона или нет"
type: docs
url: /ru/net/aspose.cells/cell/ismerged/
---
## Cell.IsMerged property

Проверяет, является ли ячейка частью объединённого диапазона.

```csharp
public bool IsMerged { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsMergedDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Объединить ячейки A1 до B2
            worksheet.Cells.Merge(0, 0, 2, 2);

            // Проверьте, объединена ли ячейка A1
            bool isMerged = worksheet.Cells["A1"].IsMerged;
            Console.WriteLine("Is cell A1 merged? " + isMerged);

            // Проверьте, объединена ли ячейка C1 (должно быть false)
            isMerged = worksheet.Cells["C1"].IsMerged;
            Console.WriteLine("Is cell C1 merged? " + isMerged);

            // Сохраните книгу
            workbook.Save("MergedCellsDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


