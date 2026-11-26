---
title: "DBConnection.ConnectionString"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DBConnection. Строка информации о соединении используется для установления контакта с источником данных OLE DB или ODBC"
type: docs
url: /ru/net/aspose.cells.externalconnections/dbconnection/connectionstring/
---
## DBConnection.ConnectionString property

Строка информации о соединении используется для установления контакта с источником данных OLE DB или ODBC.

```csharp
public override string ConnectionString { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class DBConnectionPropertyConnectionStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            try
            {
                // Получите доступ к коллекции внешних соединений
                ExternalConnectionCollection connections = workbook.DataConnections;

                // Создайте новый DBConnection, добавив его в коллекцию
                DBConnection dbConnection = (DBConnection)connections[connections.Count];

                // Отобразите начальное значение ConnectionString
                Console.WriteLine("Initial ConnectionString: " + dbConnection.ConnectionString);

                // Установите новую строку соединения
                dbConnection.ConnectionString = "Provider=Microsoft.Jet.OLEDB.4.0;Data Source=C:\\data\\database.mdb;";

                // Отобразите обновлённое значение ConnectionString
                Console.WriteLine("Updated ConnectionString: " + dbConnection.ConnectionString);

                // Сохраните книгу
                workbook.Save("ConnectionStringDemo.xlsx");
                Console.WriteLine("ConnectionString demonstration completed successfully.");
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

* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


