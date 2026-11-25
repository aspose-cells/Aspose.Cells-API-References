---
title: "ExternalConnection.Parameters"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ExternalConnection. Ottiene ConnectionParameterCollection per una query ODBC o web"
type: docs
url: /it/net/aspose.cells.externalconnections/externalconnection/parameters/
---
## ExternalConnection.Parameters property

Ottiene [`ConnectionParameterCollection`](../../connectionparametercollection/) per una query ODBC o web.

```csharp
public ConnectionParameterCollection Parameters { get; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Accedi alla prima connessione esterna (supponendo che ne esista una)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Visualizza le informazioni della raccolta Parameters
                ConnectionParameterCollection parameters = connection.Parameters;
                Console.WriteLine($"Number of parameters: {parameters.Count}");
                
                // Visualizza le informazioni di ciascun parametro, se disponibili
                foreach (ConnectionParameter param in parameters)
                {
                    Console.WriteLine($"Parameter name: {param.Name}");
                    Console.WriteLine($"Parameter type: {param.Type}");
                    Console.WriteLine($"Parameter prompt: {param.Prompt}");
                    Console.WriteLine("----------------------");
                }
                
                // Salva la cartella di lavoro
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

### Vedi anche

* class [ConnectionParameterCollection](../../connectionparametercollection/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


