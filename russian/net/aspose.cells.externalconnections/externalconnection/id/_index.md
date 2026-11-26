---
title: "ExternalConnection.Id"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ExternalConnection. Получает идентификатор соединения"
type: docs
url: /ru/net/aspose.cells.externalconnections/externalconnection/id/
---
## ExternalConnection.Id property

Получает идентификатор соединения.

```csharp
public int Id { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyIdDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            try
            {
                // Получите доступ к первому внешнему соединению (книга поставляется с соединениями по умолчанию)
                ExternalConnection connection = workbook.DataConnections[0];

                // Отобразить текущее значение Id (свойство только для чтения)
                Console.WriteLine("External Connection Id: " + connection.Id);

                // Отобразить другие свойства только для чтения для контекста
                Console.WriteLine("Connection Class Type: " + connection.ClassType);
                Console.WriteLine("Connection Name: " + connection.Name);

                // Сохраните книгу
                workbook.Save("ExternalConnectionIdDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with connection Id: " + connection.Id);
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


