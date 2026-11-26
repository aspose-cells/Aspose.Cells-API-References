---
title: "ExternalConnection.Parameters"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExternalConnection. Obtiene ConnectionParameterCollection para una consulta ODBC o web"
type: docs
url: /es/net/aspose.cells.externalconnections/externalconnection/parameters/
---
## ExternalConnection.Parameters property

Obtiene [`ConnectionParameterCollection`](../../connectionparametercollection/) para una consulta ODBC o web.

```csharp
public ConnectionParameterCollection Parameters { get; }
```

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            try
            {
                // Acceda a la primera conexión externa (suponiendo que exista una)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Mostrar la información de la colección Parameters
                ConnectionParameterCollection parameters = connection.Parameters;
                Console.WriteLine($"Number of parameters: {parameters.Count}");
                
                // Mostrar la información de cada parámetro si está disponible
                foreach (ConnectionParameter param in parameters)
                {
                    Console.WriteLine($"Parameter name: {param.Name}");
                    Console.WriteLine($"Parameter type: {param.Type}");
                    Console.WriteLine($"Parameter prompt: {param.Prompt}");
                    Console.WriteLine("----------------------");
                }
                
                // Guarda el libro de trabajo
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

### Ver también

* class [ConnectionParameterCollection](../../connectionparametercollection/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


