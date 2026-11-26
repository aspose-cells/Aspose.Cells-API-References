---
title: "DataModelConnection.ConnectionString"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DataModelConnection. Строка информации о соединении используется для установления контакта с источником данных OLE DB или ODBC"
type: docs
url: /ru/net/aspose.cells.externalconnections/datamodelconnection/connectionstring/
---
## DataModelConnection.ConnectionString property

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
    using System.Runtime.Serialization;

    public class DataModelConnectionPropertyConnectionStringDemo
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

                // Отобразить начальное значение ConnectionString (пусто)
                Console.WriteLine("Initial ConnectionString: " + connection.ConnectionString);

                // Установить свойство ConnectionString
                connection.ConnectionString = "Provider=SQLOLEDB;Data Source=Northwind;Integrated Security=SSPI";
                
                // Отобразите обновлённое значение ConnectionString
                Console.WriteLine("Updated ConnectionString: " + connection.ConnectionString);

                // Установить другие необходимые свойства для полного соединения
                connection.Command = "SELECT * FROM Customers";
                connection.CommandType = OLEDBCommandType.SqlStatement;

                // Сохранить рабочую книгу с соединением
                workbook.Save("ConnectionStringDemo.xlsx");
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


