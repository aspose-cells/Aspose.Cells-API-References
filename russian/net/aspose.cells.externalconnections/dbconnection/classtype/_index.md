---
title: "DBConnection.ClassType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DBConnection. Возвращает тип этого объекта ExternalConnection"
type: docs
url: /ru/net/aspose.cells.externalconnections/dbconnection/classtype/
---
## DBConnection.ClassType property

Возвращает тип этого [`ExternalConnection`](../../externalconnection/) объекта.

```csharp
public override ExternalConnectionClassType ClassType { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class DBConnectionPropertyClassTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            try
            {
                // Создайте новый экземпляр DBConnection, добавив его в коллекцию
                // Поскольку у DBConnection нет публичного конструктора без параметров,
                // мы позволим коллекции создать его за нас
                var connections = workbook.DataConnections;
                DBConnection dbConnection = (DBConnection)connections[connections.Count];
                
                // Отобразите значение ClassType (свойство только для чтения)
                Console.WriteLine("DBConnection ClassType: " + dbConnection.ClassType);
                
                // Продемонстрируйте установку других свойств, чтобы пример был более содержательным
                dbConnection.ConnectionString = "Server=myServerAddress;Database=myDataBase;";
                dbConnection.CommandType = OLEDBCommandType.TableName;
                dbConnection.Command = "Customers";
                
                // Сохраните книгу
                workbook.Save("DBConnectionDemo.xlsx");
                
                Console.WriteLine("ClassType demonstration completed successfully.");
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

* enum [ExternalConnectionClassType](../../externalconnectionclasstype/)
* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


