---
title: "Worksheet.ListObjects"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Worksheet property. Получает все ListObjects на этом листе"
type: docs
url: /ru/net/aspose.cells/worksheet/listobjects/
---
## Worksheet.ListObjects property

Получает все ListObjects в этом листе.

```csharp
public ListObjectCollection ListObjects { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyListObjectsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);
            
            // Создать ListObject (таблица)
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];
            table.DisplayName = "ProductTable";
            table.ShowTotals = true;
            
            // Изменить размер таблицы, чтобы включить больше строк
            table.Resize(table.StartRow, table.StartColumn, 5, table.EndColumn, true);
            
            // Добавьте больше данных в расширенную таблицу
            worksheet.Cells["A4"].PutValue("Item3");
            worksheet.Cells["B4"].PutValue(300);
            worksheet.Cells["A5"].PutValue("Item4");
            worksheet.Cells["B5"].PutValue(400);
            
            // Получите доступ к таблице через свойство ListObjects
            ListObject retrievedTable = worksheet.ListObjects["ProductTable"];
            retrievedTable.ShowHeaderRow = true;
            
            // Сохраните книгу
            workbook.Save("ListObjectsDemo.xlsx");
        }
    }
}
```

### См. также

* class [ListObjectCollection](../../../aspose.cells.tables/listobjectcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


