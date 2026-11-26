---
title: "Workbook.DataConnections"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Workbook. Возвращает коллекцию ExternalConnection"
type: docs
url: /ru/net/aspose.cells/workbook/dataconnections/
---
## Workbook.DataConnections property

Возвращает коллекцию [`ExternalConnection`](../../../aspose.cells.externalconnections/externalconnection/).

```csharp
public ExternalConnectionCollection DataConnections { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookPropertyDataConnectionsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Создайте пример рабочего листа
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые данные, чтобы пример имел смысл
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Обратитесь к свойству DataConnections
                var dataConnections = workbook.DataConnections;

                // Отобразите текущее значение свойства (операция чтения)
                Console.WriteLine("DataConnections count: " + dataConnections.Count);

                // Итерируйте по соединениям, если они существуют
                for (int i = 0; i < dataConnections.Count; i++)
                {
                    var connection = dataConnections[i];
                    Console.WriteLine($"Connection {i + 1}: {connection.Name}");
                }

                // Показать, как свойство влияет на поведение
                Console.WriteLine("DataConnections has been demonstrated");

                // Сохранить результат
                workbook.Save("DataConnectionsDemo.xlsx");
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

* class [ExternalConnectionCollection](../../../aspose.cells.externalconnections/externalconnectioncollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


