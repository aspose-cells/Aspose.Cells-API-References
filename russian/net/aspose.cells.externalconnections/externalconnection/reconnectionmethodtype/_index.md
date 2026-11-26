---
title: "ExternalConnection.ReconnectionMethodType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ExternalConnection. Указывает, что приложение таблицы должно делать при сбое соединения. Значение по умолчанию — ReConnectionMethodType.Required."
type: docs
url: /ru/net/aspose.cells.externalconnections/externalconnection/reconnectionmethodtype/
---
## ExternalConnection.ReconnectionMethodType property

Указывает, что должно делать приложение электронных таблиц при сбое соединения. Значение по умолчанию — ReConnectionMethodType.Required.

```csharp
public ReConnectionMethodType ReconnectionMethodType { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyReconnectionMethodTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            try
            {
                // Получить доступ к первому внешнему соединению (при условии, что оно существует)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Отобразить текущее значение ReconnectionMethodType
                Console.WriteLine("Initial ReconnectionMethodType: " + connection.ReconnectionMethodType);
                
                // Продемонстрировать установку свойства (поскольку оно доступно для чтения и записи).
                connection.ReconnectionMethodType = ReConnectionMethodType.Always;
                Console.WriteLine("Updated ReconnectionMethodType: " + connection.ReconnectionMethodType);
                
                // Перебрать возможные значения, чтобы продемонстрировать возможность установки
                foreach (ReConnectionMethodType method in Enum.GetValues(typeof(ReConnectionMethodType)))
                {
                    connection.ReconnectionMethodType = method;
                    Console.WriteLine($"ReconnectionMethodType set to: {method}");
                }
                
                // Сохранить книгу с изменёнными настройками соединения
                workbook.Save("ReconnectionMethodTypeDemo.xlsx");
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

* enum [ReConnectionMethodType](../../reconnectionmethodtype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


