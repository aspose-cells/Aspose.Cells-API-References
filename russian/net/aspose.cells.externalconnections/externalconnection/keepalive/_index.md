---
title: "ExternalConnection.KeepAlive"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ExternalConnection. True, когда приложение электронных таблиц должно прилагать усилия для поддержания соединения открытым. Когда false, приложение должно закрыть соединение после получения информации"
type: docs
url: /ru/net/aspose.cells.externalconnections/externalconnection/keepalive/
---
## ExternalConnection.KeepAlive property

True, когда приложение электронных таблиц должно стараться держать соединение открытым. При false приложение должно закрыть соединение после получения информации.

```csharp
public bool KeepAlive { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyKeepAliveDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            try
            {
                // Получить доступ к первому внешнему соединению (при условии, что оно существует)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Отобразить текущее значение KeepAlive
                Console.WriteLine("Initial KeepAlive value: " + connection.KeepAlive);
                
                // Переключить значение KeepAlive, так как оно доступно для чтения и записи
                connection.KeepAlive = !connection.KeepAlive;
                Console.WriteLine("Updated KeepAlive value: " + connection.KeepAlive);
                
                // Сохранить книгу с изменёнными настройками соединения
                workbook.Save("KeepAliveDemo.xlsx");
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


