---
title: "Column.IsHidden"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Column. Указывает, скрыт ли столбец"
type: docs
url: /ru/net/aspose.cells/column/ishidden/
---
## Column.IsHidden property

Указывает, скрыт ли столбец.

```csharp
public bool IsHidden { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnPropertyIsHiddenDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установить ширину столбца для демонстрации
            worksheet.Cells.Columns[1].Width = 20;
            Console.WriteLine("Column 1 width before hiding: " + worksheet.Cells.Columns[1].Width);

            // Скрыть столбец
            worksheet.Cells.Columns[1].IsHidden = true;
            Console.WriteLine("Column 1 is hidden: " + worksheet.Cells.Columns[1].IsHidden);

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


