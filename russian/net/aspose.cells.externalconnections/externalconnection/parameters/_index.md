---
title: "ExternalConnection.Parameters"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ExternalConnection. Получает ConnectionParameterCollection для ODBC или веб‑запроса"
type: docs
url: /ru/net/aspose.cells.externalconnections/externalconnection/parameters/
---
## ExternalConnection.Parameters property

Получает [`ConnectionParameterCollection`](../../connectionparametercollection/) для ODBC или веб‑запроса.

```csharp
public ConnectionParameterCollection Parameters { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyParametersDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            try
            {
                // Получить доступ к первому внешнему соединению (при условии, что оно существует)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Отобразить информацию о коллекции Parameters
                ConnectionParameterCollection parameters = connection.Parameters;
                Console.WriteLine($"Number of parameters: {parameters.Count}");
                
                // Отобразить информацию о каждом параметре, если доступна
                foreach (ConnectionParameter param in parameters)
                {
                    Console.WriteLine($"Parameter name: {param.Name}");
                    Console.WriteLine($"Parameter type: {param.Type}");
                    Console.WriteLine($"Parameter prompt: {param.Prompt}");
                    Console.WriteLine("----------------------");
                }
                
                // Сохраните книгу
                workbook.Save("ParametersDemo.xlsx");
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

* class [ConnectionParameterCollection](../../connectionparametercollection/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


