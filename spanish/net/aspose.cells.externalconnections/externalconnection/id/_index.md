---
title: "ExternalConnection.Id"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "ExternalConnection property. Obtiene el id de la conexión"
type: docs
url: /es/net/aspose.cells.externalconnections/externalconnection/id/
---
## ExternalConnection.Id property

Obtiene el id de la conexión.

```csharp
public int Id { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyIdDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            try
            {
                // Acceder a la primera conexión externa (el libro de trabajo viene con conexiones predeterminadas)
                ExternalConnection connection = workbook.DataConnections[0];

                // Mostrar el valor actual de Id (propiedad de solo lectura)
                Console.WriteLine("External Connection Id: " + connection.Id);

                // Mostrar otras propiedades de solo lectura para contexto
                Console.WriteLine("Connection Class Type: " + connection.ClassType);
                Console.WriteLine("Connection Name: " + connection.Name);

                // Guarda el libro de trabajo
                workbook.Save("ExternalConnectionIdDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with connection Id: " + connection.Id);
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

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


