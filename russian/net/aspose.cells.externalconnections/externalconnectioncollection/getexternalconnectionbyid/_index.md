---
title: "ExternalConnectionCollection.GetExternalConnectionById"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ExternalConnectionCollection. Получает элемент ExternalConnection с указанным идентификатором"
type: docs
url: /ru/net/aspose.cells.externalconnections/externalconnectioncollection/getexternalconnectionbyid/
---
## ExternalConnectionCollection.GetExternalConnectionById method

Получает элемент [`ExternalConnection`](../../externalconnection/) с указанным идентификатором.

```csharp
public ExternalConnection GetExternalConnectionById(int connId)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| connId | Int32 | идентификатор внешнего соединения |

### Возвращаемое значение

Элемент с указанным идентификатором.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class ExternalConnectionCollectionMethodGetExternalConnectionByIdWithInt32Demo
    {
        public static void Run()
        {
            // Создать новую рабочую книгу с образцами подключений данных
            Workbook workbook = new Workbook();
            
            // Получить коллекцию внешних подключений
            ExternalConnectionCollection dataConns = workbook.DataConnections;

            // Создавать и добавлять подключения, используя правильные методы API
            // Примечание: При реальном использовании обычно получают существующие подключения
            // а не создавая новые таким способом
            int connectionId1 = 1;
            int connectionId2 = 2;
            
            // Получить конкретное подключение по ID (изначально будет null)
            ExternalConnection specificConn = dataConns.GetExternalConnectionById(connectionId1);
            
            if (specificConn == null)
            {
                Console.WriteLine($"No connection found with ID {connectionId1}");
                // При реальном использовании вы будете работать с существующими подключениями
                // или создавать их через правильные методы API
            }
            else
            {
                Console.WriteLine($"Found connection: ID={specificConn.ConnectionId}, Name={specificConn.Name}");
                specificConn.Name = "ModifiedConnection";
            }

            // Сохраните книгу
            workbook.Save("ExternalConnectionDemo.xlsx");
        }
    }
}
```

### См. также

* class [ExternalConnection](../../externalconnection/)
* class [ExternalConnectionCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


