---
title: "Row.IsCollapsed"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Row. указывает, свернута ли строка"
type: docs
url: /ru/net/aspose.cells/row/iscollapsed/
---
## Row.IsCollapsed property

является ли строка свернутой

```csharp
public bool IsCollapsed { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyIsCollapsedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте и стилизуйте строку
            Row row = worksheet.Cells.Rows[0];
            row.Height = 20;
            row.GroupLevel = 1;
            
            // Продемонстрируйте свойство IsCollapsed
            row.IsCollapsed = true;
            Console.WriteLine("Row is collapsed: " + row.IsCollapsed);

            // Разверните строку
            row.IsCollapsed = false;
            Console.WriteLine("Row is collapsed: " + row.IsCollapsed);

            // Сохраните книгу
            workbook.Save("RowIsCollapsedDemo.xlsx");
        }
    }
}
```

### См. также

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


