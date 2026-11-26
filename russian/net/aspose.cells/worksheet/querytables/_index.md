---
title: "Worksheet.QueryTables"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Получает QueryTableCollection в рабочем листе"
type: docs
url: /ru/net/aspose.cells/worksheet/querytables/
---
## Worksheet.QueryTables property

Получает [`QueryTableCollection`](../../querytablecollection/) в рабочем листе.

```csharp
public QueryTableCollection QueryTables { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyQueryTablesDemo
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
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1.8);
            
            // Получить первую таблицу запросов (поскольку мы не можем добавить новые напрямую)
            // Примечание: коллекция QueryTables доступна только для чтения в этой версии API
            if (worksheet.QueryTables.Count > 0)
            {
                QueryTable queryTable = worksheet.QueryTables[0];
                
                // Отобразить информацию о таблице запросов
                Console.WriteLine("Query Table Name: " + queryTable.Name);
                Console.WriteLine("Result Range: " + queryTable.ResultRange.Address);
                Console.WriteLine("Number of Query Tables: " + worksheet.QueryTables.Count);
            }
            else
            {
                Console.WriteLine("No query tables found in the worksheet.");
            }
            
            // Сохраните книгу
            workbook.Save("QueryTableDemo.xlsx");
        }
    }
}
```

### См. также

* class [QueryTableCollection](../../querytablecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


