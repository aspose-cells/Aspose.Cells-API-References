---
title: "ExternalConnection.Parameters"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExternalConnection-egenskap. Hämtar ConnectionParameterCollection för en ODBC‑ eller webbfråga"
type: docs
url: /sv/net/aspose.cells.externalconnections/externalconnection/parameters/
---
## ExternalConnection.Parameters property

Hämtar [`ConnectionParameterCollection`](../../connectionparametercollection/) för en ODBC‑ eller webbfråga.

```csharp
public ConnectionParameterCollection Parameters { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            try
            {
                // Åtkomst till den första externa anslutningen (förutsatt att en sådan finns)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Visa information om Parameters‑samlingen
                ConnectionParameterCollection parameters = connection.Parameters;
                Console.WriteLine($"Number of parameters: {parameters.Count}");
                
                // Visa information om varje parameter om den finns tillgänglig
                foreach (ConnectionParameter param in parameters)
                {
                    Console.WriteLine($"Parameter name: {param.Name}");
                    Console.WriteLine($"Parameter type: {param.Type}");
                    Console.WriteLine($"Parameter prompt: {param.Prompt}");
                    Console.WriteLine("----------------------");
                }
                
                // Spara arbetsboken
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

### Se även

* class [ConnectionParameterCollection](../../connectionparametercollection/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


