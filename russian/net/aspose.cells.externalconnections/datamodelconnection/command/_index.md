---
title: "DataModelConnection.Command"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DataModelConnection. Строка, содержащая команду базы данных, которую необходимо передать API поставщика данных, который будет взаимодействовать с внешним источником для получения данных"
type: docs
url: /ru/net/aspose.cells.externalconnections/datamodelconnection/command/
---
## DataModelConnection.Command property

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
    using System.Runtime.Serialization;

    public class DataModelConnectionPropertyCommandDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            try
            {
                // Создать экземпляр DataModelConnection, используя неинициализированный объект
                DataModelConnection connection = (DataModelConnection)FormatterServices.GetUninitializedObject(typeof(DataModelConnection));
                ((IList<ExternalConnection>)workbook.DataConnections).Add(connection);

                // Отобразить начальное значение Command (пусто)
                Console.WriteLine("Initial Command: " + connection.Command);

                // Установить свойство Command
                connection.Command = "SELECT * FROM Customers";
                
                // Отобразить обновленное значение Command
                Console.WriteLine("Updated Command: " + connection.Command);

                // Установить другие необходимые свойства для полного соединения
                connection.CommandType = OLEDBCommandType.SqlStatement;
                connection.ConnectionString = "Provider=SQLOLEDB;Data Source=Northwind;Integrated Security=SSPI";

                // Сохранить рабочую книгу с соединением
                workbook.Save("CommandDemo.xlsx");
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

* class [DataModelConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


