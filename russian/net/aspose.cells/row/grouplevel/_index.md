---
title: "Row.GroupLevel"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Row. Возвращает уровень группировки строки"
type: docs
url: /ru/net/aspose.cells/row/grouplevel/
---
## Row.GroupLevel property

Получает уровень группы строки.

```csharp
public byte GroupLevel { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyGroupLevelDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Группировать строки 4‑6 (hidden = false)
            worksheet.Cells.GroupRows(3, 5, false);

            // Получить уровень группировки строки 4
            int groupLevel = worksheet.Cells.Rows[3].GroupLevel;
            Console.WriteLine("Group level of row 4: " + groupLevel);

            // Разгруппировать строки
            worksheet.Cells.UngroupRows(3, 5);
        }
    }
}
```

### См. также

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


