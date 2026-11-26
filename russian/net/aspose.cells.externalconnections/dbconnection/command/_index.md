---
title: "DBConnection.Command"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DBConnection. Строка, содержащая команду базы данных, которую следует передать API поставщика данных, взаимодействующего с внешним источником для получения данных"
type: docs
url: /ru/net/aspose.cells.externalconnections/dbconnection/command/
---
## DBConnection.Command property

Строка, содержащая команду базы данных, передаваемую API поставщика данных, который будет взаимодействовать с внешним источником для получения данных

```csharp
public override string Command { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class DBConnectionPropertyCommandDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            try
            {
                // Получите доступ к коллекции внешних соединений
                ExternalConnectionCollection connections = workbook.DataConnections;

                // Найдите первое DBConnection в коллекции (если есть)
                DBConnection dbConn = null;
                foreach (ExternalConnection conn in connections)
                {
                    if (conn is DBConnection dbConnection)
                    {
                        dbConn = dbConnection;
                        break;
                    }
                }

                if (dbConn == null)
                {
                    Console.WriteLine("No DBConnection objects found in the workbook.");
                }
                else
                {
                    // Отобразить текущее значение Command (операция чтения)
                    Console.WriteLine("Current Command: " + dbConn.Command);

                    // Продемонстрировать установку Command (свойство чтения‑записи)
                    dbConn.Command = "SELECT * FROM Customers";
                    Console.WriteLine("Updated Command: " + dbConn.Command);
                }

                // Сохраните книгу
                workbook.Save("CommandDemo.xlsx");
                Console.WriteLine("Workbook saved as CommandDemo.xlsx");
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


