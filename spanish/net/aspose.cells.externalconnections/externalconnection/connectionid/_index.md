---
title: "ExternalConnection.ConnectionId"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExternalConnection. Especifica el identificador único de esta conexión"
type: docs
url: /es/net/aspose.cells.externalconnections/externalconnection/connectionid/
---
## ExternalConnection.ConnectionId property

Especifica el identificador único de esta conexión.

```csharp
[Obsolete("Use ExternalConnection.Id property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int ConnectionId { get; }
```

### Observaciones

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad ExternalConnection.Id. Esta propiedad será eliminada 12 meses después, a partir de octubre de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyConnectionIdDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            try
            {
                // Acceder a la primera conexión externa (el libro de trabajo viene con conexiones predeterminadas)
                ExternalConnection connection = workbook.DataConnections[0];

                // Mostrar el valor ConnectionId (propiedad de solo lectura)
                Console.WriteLine("ConnectionId value: " + connection.ConnectionId);

                // Mostrar el valor Id para comparación (también de solo lectura)
                Console.WriteLine("Id value: " + connection.Id);

                // Mostrar que ambas propiedades son de solo lectura intentando mostrarlas
                Console.WriteLine("ConnectionId and Id are both read-only properties");
                Console.WriteLine("ConnectionId: " + connection.ConnectionId + ", Id: " + connection.Id);

                // Guarda el libro de trabajo
                workbook.Save("ConnectionIdDemo.xlsx");
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


