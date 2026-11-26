---
title: "Cells.IsDefaultRowHeightMatched"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cells. Указывает, что высота строки соответствует высоте шрифта по умолчанию"
type: docs
url: /ru/net/aspose.cells/cells/isdefaultrowheightmatched/
---
## Cells.IsDefaultRowHeightMatched property

Указывает, что высота строки и высота шрифта по умолчанию совпадают.

```csharp
public bool IsDefaultRowHeightMatched { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyIsDefaultRowHeightMatchedDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Установить и продемонстрировать свойство IsDefaultRowHeightMatched
            cells.IsDefaultRowHeightMatched = true;
            Console.WriteLine("IsDefaultRowHeightMatched: " + cells.IsDefaultRowHeightMatched);

            // Сохраните книгу
            workbook.Save("output.xlsx");

            // Загрузить сохранённую книгу, чтобы проверить свойство
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Cells loadedCells = loadedWorkbook.Worksheets[0].Cells;
            Console.WriteLine("Loaded IsDefaultRowHeightMatched: " + loadedCells.IsDefaultRowHeightMatched);
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


