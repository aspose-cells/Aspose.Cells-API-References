---
title: "Cell.GetTable"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cell. Получает таблицу, содержащую эту ячейку"
type: docs
url: /ru/net/aspose.cells/cell/gettable/
---
## Cell.GetTable method

Получает таблицу, содержащую эту ячейку.

```csharp
public ListObject GetTable()
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class CellMethodGetTableDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Создайте таблицу с заголовками и данными
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Price");
            cells["A2"].PutValue("Apple");
            cells["B2"].PutValue(2.5);
            cells["A3"].PutValue("Orange");
            cells["B3"].PutValue(1.8);

            // Создайте ListObject (таблицу) из диапазона данных
            int tableIndex = worksheet.ListObjects.Add("A1", "B3", true);
            ListObject table = worksheet.ListObjects[tableIndex];

            // Продемонстрируйте метод GetTable
            Cell cellInTable = cells["B2"];
            ListObject resultTable = cellInTable.GetTable();
            
            Console.WriteLine("Table found: " + (resultTable != null));
            Console.WriteLine("Table range: " + resultTable.StartRow + "," + resultTable.StartColumn + 
                            " to " + resultTable.EndRow + "," + resultTable.EndColumn);
        }
    }
}
```

### См. также

* class [ListObject](../../../aspose.cells.tables/listobject/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


