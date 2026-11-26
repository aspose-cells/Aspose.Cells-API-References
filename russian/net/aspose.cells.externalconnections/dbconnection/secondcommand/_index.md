---
title: "DBConnection.SecondCommand"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DBConnection. Указывает вторую строку текста команды, которая сохраняется при использовании полей страниц PivotTable на основе сервера. Для ODBC‑соединений serverCommand обычно представляет более широкий запрос, чем command, в первом нет условия WHERE. На основе этих двух команд Command и ServerCommand пользовательский интерфейс параметров может быть заполнен, и могут быть построены параметризованные запросы."
type: docs
url: /ru/net/aspose.cells.externalconnections/dbconnection/secondcommand/
---
## DBConnection.SecondCommand property

Указывает вторую строку команды, которая сохраняется, когда используются полевые элементы PivotTable на основе сервера. Для ODBC‑подключений serverCommand обычно представляет более широкий запрос, чем command (в первом нет предложения WHERE). На основе этих двух команд (Command и ServerCommand) можно заполнить пользовательский интерфейс параметров и построить параметризованные запросы.

```csharp
public override string SecondCommand { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class DBConnectionPropertySecondCommandDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            try
            {
                // Создайте новый экземпляр DBConnection, добавив его в коллекцию
                var connections = workbook.DataConnections;
                DBConnection dbConnection = (DBConnection)connections[0];
                
                // Настройте базовое соединение
                dbConnection.ConnectionString = "Server=myServer;Database=myDB;";
                dbConnection.CommandType = OLEDBCommandType.SqlStatement;
                dbConnection.Command = "SELECT * FROM Customers WHERE Country = 'USA'";
                
                // Установите и продемонстрируйте свойство SecondCommand
                dbConnection.SecondCommand = "SELECT * FROM Customers";
                Console.WriteLine("SecondCommand value: " + dbConnection.SecondCommand);
                
                // Измените SecondCommand, чтобы показать, что оно доступно для записи
                dbConnection.SecondCommand = "SELECT * FROM Orders";
                Console.WriteLine("Updated SecondCommand value: " + dbConnection.SecondCommand);
                
                // Сохраните книгу
                workbook.Save("SecondCommandDemo.xlsx");
                
                Console.WriteLine("SecondCommand demonstration completed successfully.");
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


