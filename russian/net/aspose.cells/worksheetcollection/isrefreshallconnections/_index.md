---
title: "WorksheetCollection.IsRefreshAllConnections"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorksheetCollection. Указывает, следует ли обновлять все соединения при открытии файла в MS Excel"
type: docs
url: /ru/net/aspose.cells/worksheetcollection/isrefreshallconnections/
---
## WorksheetCollection.IsRefreshAllConnections property

Указывает, следует ли обновлять все соединения при открытии файла в MS Excel.

```csharp
public bool IsRefreshAllConnections { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyIsRefreshAllConnectionsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к коллекции листов
            WorksheetCollection worksheets = workbook.Worksheets;
            
            // Добавить несколько примерных листов
            worksheets.Add("Sheet1");
            worksheets.Add("Sheet2");
            
            // Установить свойство IsRefreshAllConnections
            worksheets.IsRefreshAllConnections = true;
            
            // Отобразить текущее значение IsRefreshAllConnections
            Console.WriteLine("IsRefreshAllConnections: " + worksheets.IsRefreshAllConnections);
            
            // Сохраните книгу
            workbook.Save("WorksheetCollectionPropertyIsRefreshAllConnectionsDemo.xlsx");
        }
    }
}
```

### См. также

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


