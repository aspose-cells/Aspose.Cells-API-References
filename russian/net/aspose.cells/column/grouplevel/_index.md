---
title: "Column.GroupLevel"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Column. Возвращает уровень группировки колонки"
type: docs
url: /ru/net/aspose.cells/column/grouplevel/
---
## Column.GroupLevel property

Получает уровень группы столбца.

```csharp
public byte GroupLevel { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnPropertyGroupLevelDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Группировать колонки (параметр isHidden установлен в false)
            worksheet.Cells.GroupColumns(0, 2, false);
            
            // Получить уровень группировки первой колонки
            int groupLevel = worksheet.Cells.Columns[0].GroupLevel;
            
            // Вывести уровень группировки
            Console.WriteLine("Group level of first column: " + groupLevel);
            
            // Сохраните книгу
            workbook.Save("GroupLevelDemo.xlsx");
        }
    }
}
```

### См. также

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


