---
title: "ListColumn.Formula"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ListColumn. Получает и задает формулу столбца списка"
type: docs
url: /ru/net/aspose.cells.tables/listcolumn/formula/
---
## ListColumn.Formula property

Получает и задает формулу столбца списка.

```csharp
public string Formula { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnPropertyFormulaDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Создайте примерные данные и таблицу
            sheet.Cells["A1"].PutValue("Numbers");
            sheet.Cells["A2"].PutValue(5);
            sheet.Cells["A3"].PutValue(10);
            sheet.Cells["A4"].PutValue(15);
            
            sheet.Cells["B1"].PutValue("Doubled");
            sheet.Cells["B2"].PutValue("=A2*2");
            
            int tableIndex = sheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = sheet.ListObjects[tableIndex];
            table.ShowTotals = true;
            
            // Добавить формулу в столбец списка
            ListColumn column = table.ListColumns[0];
            column.Formula = "=A2*3"; // This will apply to all cells in the column
            
            // Сохраните книгу
            workbook.Save("ListColumnFormulaDemo.xlsx");
        }
    }
}
```

### См. также

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


