---
title: "ExternalConnection.ReconnectionMethod"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ExternalConnection. Указывает, что приложение таблицы должно делать при сбое соединения. Значение по умолчанию — ReConnectionMethodType.Required."
type: docs
url: /ru/net/aspose.cells.externalconnections/externalconnection/reconnectionmethod/
---
## ExternalConnection.ReconnectionMethod property

Указывает, что должно делать приложение электронных таблиц при сбое соединения. Значение по умолчанию — ReConnectionMethodType.Required.

```csharp
[Obsolete("Use ExternalConnection.ReconnectionMethodType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ReConnectionMethodType ReconnectionMethod { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство ExternalConnection.ReconnectionMethodType. Это свойство будет удалено через 12 месяцев, начиная с октября 2017 года. Aspose приносит извинения за любые причинённые неудобства.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyReconnectionMethodDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            try
            {
                // Получить доступ к первому внешнему соединению (при условии, что оно существует)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Отобразить текущее значение ReconnectionMethod (операция чтения)
                Console.WriteLine("Initial ReconnectionMethod value: " + connection.ReconnectionMethod);
                
                // Установить новые значения ReconnectionMethod (поскольку свойство доступно для чтения и записи)
                connection.ReconnectionMethod = ReConnectionMethodType.Always;
                Console.WriteLine("Updated ReconnectionMethod value: " + connection.ReconnectionMethod);
                
                connection.ReconnectionMethod = ReConnectionMethodType.Never;
                Console.WriteLine("Updated ReconnectionMethod value: " + connection.ReconnectionMethod);
                
                // Сбросить к значению по умолчанию
                connection.ReconnectionMethod = ReConnectionMethodType.Required;
                Console.WriteLine("Reset ReconnectionMethod value: " + connection.ReconnectionMethod);
                
                // Сохранить книгу с изменёнными настройками соединения
                workbook.Save("ReconnectionMethodDemo.xlsx");
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


