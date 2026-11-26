---
title: "Workbook.DataConnections"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad del libro de trabajo. Obtiene la colección ExternalConnection"
type: docs
url: /es/net/aspose.cells/workbook/dataconnections/
---
## Workbook.DataConnections property

Obtiene la colección [`ExternalConnection`](../../../aspose.cells.externalconnections/externalconnection/).

```csharp
public ExternalConnectionCollection DataConnections { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookPropertyDataConnectionsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Crear una hoja de cálculo de ejemplo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos para que el ejemplo tenga sentido
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Acceda a la propiedad DataConnections
                var dataConnections = workbook.DataConnections;

                // Muestre el valor actual de la propiedad (operación de lectura)
                Console.WriteLine("DataConnections count: " + dataConnections.Count);

                // Itere a través de las conexiones si existen
                for (int i = 0; i < dataConnections.Count; i++)
                {
                    var connection = dataConnections[i];
                    Console.WriteLine($"Connection {i + 1}: {connection.Name}");
                }

                // Mostrar cómo la propiedad afecta el comportamiento
                Console.WriteLine("DataConnections has been demonstrated");

                // Guardar el resultado
                workbook.Save("DataConnectionsDemo.xlsx");
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

* class [ExternalConnectionCollection](../../../aspose.cells.externalconnections/externalconnectioncollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


