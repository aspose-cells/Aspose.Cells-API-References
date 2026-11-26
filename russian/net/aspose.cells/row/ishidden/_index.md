---
title: "Row.IsHidden"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Row. Указывает, скрыта ли строка"
type: docs
url: /ru/net/aspose.cells/row/ishidden/
---
## Row.IsHidden property

Указывает, скрыта ли строка.

```csharp
public bool IsHidden { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyIsHiddenDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Добавьте примерные данные
            for (int i = 0; i < 10; i++)
            {
                cells[$"A{i + 1}"].PutValue($"Row {i + 1}");
            }

            // Скрыть некоторые строки
            cells.HideRow(2);  // Row 3 (0-based index 2)
            cells.HideRow(5);  // Row 6 (0-based index 5)
            cells.HideRow(8);  // Row 9 (0-based index 8)

            // Проверьте и отобразите статус IsHidden для каждой строки
            for (int i = 0; i < 10; i++)
            {
                bool isHidden = cells.Rows[i].IsHidden;
                Console.WriteLine($"Row {i + 1} is hidden: {isHidden}");
            }

            // Сохраните книгу
            workbook.Save("RowHiddenDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


