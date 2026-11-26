---
title: "Класс QueryTable"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.QueryTable. Представляет информацию о QueryTable."
type: docs
url: /ru/net/aspose.cells/querytable/
---
## QueryTable class

Представляет информацию о QueryTable.

```csharp
public class QueryTable
```

## Свойства

| Имя | Описание |
| --- | --- |
| [AdjustColumnWidth](../../aspose.cells/querytable/adjustcolumnwidth/) { get; set; } | Возвращает или задает AdjustColumnWidth объекта. |
| [ConnectionId](../../aspose.cells/querytable/connectionid/) { get; } | Получает идентификатор соединения query table. |
| [ExternalConnection](../../aspose.cells/querytable/externalconnection/) { get; } | Получает связанное внешнее соединение. |
| [Name](../../aspose.cells/querytable/name/) { get; } | Получает имя querytable. |
| [PreserveFormatting](../../aspose.cells/querytable/preserveformatting/) { get; set; } | Возвращает или задает PreserveFormatting объекта. |
| [ResultRange](../../aspose.cells/querytable/resultrange/) { get; } | Получает диапазон результата. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassQueryTableDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для создания query table (симуляция внешних данных)
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Mary");
            
            // Проверить, есть ли какие‑либо query tables в листе
            if (worksheet.QueryTables.Count > 0)
            {
                // Получить первую query table
                QueryTable qt = worksheet.QueryTables[0];
                
                // Отобразить свойства таблицы запросов
                Console.WriteLine("Query Table Name: " + qt.Name);
                Console.WriteLine("Connection ID: " + qt.ConnectionId);
                Console.WriteLine("Result Range: " + qt.ResultRange.Address);
                Console.WriteLine("Preserve Formatting: " + qt.PreserveFormatting);
                Console.WriteLine("Adjust Column Width: " + qt.AdjustColumnWidth);
                
                // Изменить некоторые свойства
                qt.PreserveFormatting = true;
                qt.AdjustColumnWidth = false;
            }
            else
            {
                Console.WriteLine("No query tables found in the worksheet.");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


