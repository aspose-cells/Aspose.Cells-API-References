---
title: "ExternalConnection.BackgroundRefresh"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ExternalConnection. Указывает, может ли соединение обновляться в фоновом режиме асинхронно. true, если предпочтительно обновлять соединение асинхронно в фоне; false, если предпочтительно обновлять соединение синхронно в переднем плане."
type: docs
url: /ru/net/aspose.cells.externalconnections/externalconnection/backgroundrefresh/
---
## ExternalConnection.BackgroundRefresh property

Указывает, может ли соединение обновляться в фоновом режиме (асинхронно). true, если предпочтительно обновлять соединение асинхронно в фоне; false, если предпочтительно обновлять соединение синхронно в переднем плане.

```csharp
public bool BackgroundRefresh { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyBackgroundRefreshDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            try
            {
                // Получить доступ к первому внешнему соединению (при условии, что оно существует)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Отобразить текущее значение BackgroundRefresh
                Console.WriteLine("Initial BackgroundRefresh value: " + connection.BackgroundRefresh);
                
                // Переключить значение BackgroundRefresh
                connection.BackgroundRefresh = !connection.BackgroundRefresh;
                Console.WriteLine("Updated BackgroundRefresh value: " + connection.BackgroundRefresh);
                
                // Сохранить книгу с изменёнными настройками соединения
                workbook.Save("BackgroundRefreshDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


