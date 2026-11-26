---
title: "ExternalConnection.ConnectionId"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ExternalConnection. Указывает уникальный идентификатор этого соединения"
type: docs
url: /ru/net/aspose.cells.externalconnections/externalconnection/connectionid/
---
## ExternalConnection.ConnectionId property

Указывает уникальный идентификатор этого соединения.

```csharp
[Obsolete("Use ExternalConnection.Id property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int ConnectionId { get; }
```

### Примечания

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство ExternalConnection.Id. Это свойство будет удалено через 12 месяцев, начиная с октября 2024 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyConnectionIdDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            try
            {
                // Получите доступ к первому внешнему соединению (книга поставляется с соединениями по умолчанию)
                ExternalConnection connection = workbook.DataConnections[0];

                // Отобразить значение ConnectionId (свойство только для чтения)
                Console.WriteLine("ConnectionId value: " + connection.ConnectionId);

                // Отобразить значение Id для сравнения (также только для чтения)
                Console.WriteLine("Id value: " + connection.Id);

                // Показать, что оба свойства только для чтения, попытавшись отобразить их
                Console.WriteLine("ConnectionId and Id are both read-only properties");
                Console.WriteLine("ConnectionId: " + connection.ConnectionId + ", Id: " + connection.Id);

                // Сохраните книгу
                workbook.Save("ConnectionIdDemo.xlsx");
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


